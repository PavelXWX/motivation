<script>
  import ArticleLinkBg from "./ArticleLinkBg.svelte";
  import ArticleHeaderBg from "./ArticleHeaderBg.svelte";
  import ArticleFooterBg from "./ArticleFooterBg.svelte";
  export let ArtMark = 0
  export let ArtComments = 0
  export let ArtTitle = ""
  export let ArtText =""
  export let ArtImg =""
</script>

<div class="Modal" style="background: url({ArtImg}); background-size: cover; background-blend-mode: multiply;">

  <ArticleHeaderBg/>
  <ArticleLinkBg ArtTitle={ArtTitle} ArtText={ArtText}/> 
  <ArticleFooterBg ArtMark={ArtMark} ArtComments={ArtComments}/>               
</div>


<style>
  .Modal {
    width: 100%;
    border-radius: 10px;
    margin: 0 auto;
    padding: 20px 30px 20px 30px;
    display: flex;
    flex-direction: column;
    gap: 20px;
    box-shadow: inset 0 0 0 2000px rgba(0, 0, 0, 0.498);
    
    /* opacity: 0.6; */
  }

</style>