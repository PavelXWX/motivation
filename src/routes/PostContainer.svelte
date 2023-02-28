<script>
  import Article from "./Article.svelte";
  import "../posts.js" 
  // import { Posts } from "../posts.js";
  import PostButtons from "./PostButtons.svelte";
  import ArticleBg from "./ArticleBg.svelte";
  import ArticleBot from "./ArticleBot.svelte";


</script>

<div class="Modal">
  <PostButtons/> 
  <!-- {#each Posts as item}
 
  <Article ArtTitle={item.title} ArtText={item.text} ArtImg={item.img} ArtComments={item.comments} ArtMark={item.mark}/> 
  <ArticleBg ArtTitle={item.title} ArtText={item.text} ArtImg={item.img} ArtComments={item.comments} ArtMark={item.mark}/>
  <ArticleBot ArtTitle={item.title} ArtText={item.text} ArtImg={item.img} ArtComments={item.comments} ArtMark={item.mark}/>
  {/each} -->

 
         
</div>


<style>
  .Modal {
    background-color: rgb(230, 228, 228);
    width: 920px;
    margin: 0 auto;
    padding: 100px 40px 40px 40px;
    display: flex;
    flex-direction: column;
    gap: 30px;
    min-width: 380px;
  }
  @media screen and (max-width:1720px) {
    .Modal {
      background-color: rgb(230, 228, 228);
      width: 920px;
      margin: 0 400px auto auto;
      padding: 100px 40px 40px 40px;
      display: flex;
      flex-direction: column;
      gap: 30px;
    }
  }
  @media screen and (max-width:1550px) {
    .Modal {
      width: 920px;
      margin: 0 270px auto auto;
    }
  }
  @media screen and (max-width:1435px) {
    .Modal {
      width: 880px;
      margin: 0 270px auto auto;
    }
  }
  @media screen and (max-width:1394px) {
    .Modal {
      width: 840px;
      margin: 0 270px auto auto;
    }
  }
  @media screen and (max-width:1310px) {
    .Modal {
      width: 800px;
      margin: 0 270px auto auto;
    }
  }
  @media screen and (max-width:1280px) {
    .Modal {
      width: 760px;
      margin: 0 270px auto auto;
    }
  }
  @media screen and (max-width:1230px) {
    .Modal {
      width: 720px;
      margin: 0 270px auto auto;
    }
  }
  @media screen and (max-width:1200px) {
    .Modal {
      width: 920px;
      margin: 0 auto 0 0
    }
  }
  @media screen and (max-width:1180px) {
    .Modal {
      width: 880px;
      margin: 0 auto 0 0
    }
  }
  @media screen and (max-width:1140px) {
    .Modal {
      width: 820px;
      margin: 0 auto 0 0
    }
  }
  @media screen and (max-width:1100px) {
    .Modal {
      width: 780px;
      margin: 0 auto 0 0
    }
  }
  @media screen and (max-width:1050px) {
    .Modal {
      width: 740px;
      margin: 0 auto 0 -10px
    }
  }
  @media screen and (max-width:1000px) {
    .Modal {
      width: 740px;
    }
  }
  @media screen and (max-width:950px) {
    .Modal {
      width: 840px;
      margin: 0 auto 
    }
  }
  @media screen and (max-width:850px) {
    .Modal {
      width: 100%;
      margin: 0 auto 
    }
  }
</style>