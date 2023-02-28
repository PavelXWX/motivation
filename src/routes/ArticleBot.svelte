<script>
  import ArticleLinkBot from "./ArticleLinkBot.svelte";
  import ArticleHeader from "./ArticleHeader.svelte";
  import ArticleFooter from "./ArticleFooter.svelte";
  export let ArtMark = 0
  export let ArtComments = 0
  export let ArtTitle = ""
  export let ArtText =""
  export let ArtImg =""
</script>

<div class="Modal">
  <ArticleHeader/>
  <ArticleLinkBot ArtTitle={ArtTitle} ArtText={ArtText} ArtImg={ArtImg}/> 
  <ArticleFooter ArtMark={ArtMark} ArtComments={ArtComments}/>               
</div>


<style>
  .Modal {
    background-color: rgb(222, 239, 239);
    width: 100%;
    border-radius: 10px;
    margin: 0 auto;
    padding: 20px 30px 20px 30px;
    display: flex;
    flex-direction: column;
    gap: 20px;
  }

</style>