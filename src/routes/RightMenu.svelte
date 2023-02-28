<script>
  import AudioPlayer from './AudioPlayer.svelte'
  import Top from './Top.svelte';
  let src = 'https://sveltejs.github.io/assets/music/strauss.mp3'
</script>

<div class="rightmenu"> 
  <div class="music">
    <h2 class="rightmenu-item">Музыка для мотивации</h2>
    <AudioPlayer {src} />
  </div>
  <div class="top">
    <h2 class="top-item">Самый топ</h2>
    <Top/>
  </div>
  

</div>



<style>
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap');
  .rightmenu {
    /* background-color: rgb(242, 242, 242); */
    /* width: 500; */
    border-radius: 0 10px 10px 0;
    margin: 65px 0 0 0 ;
    padding: 40px 40px 40px 40px;
    display: flex;
    position: fixed;
    flex-direction: column;
    gap: 40px; 
    right: 0;
  }
  .music {
    background-color: rgb(222, 239, 239);
    padding: 20px;
    border-radius: 10px;
    margin: 0 ;
    display: flex;
    flex-direction: column;
    gap: 20px; 
  }
  .top {
    background-color: rgb(222, 239, 239);
    padding: 20px;
    border-radius: 10px;
    margin: 0 ;
    display: flex;
    flex-direction: column;
    gap: 20px; 
  }
  .top:hover {
    background-color: rgba(199, 232, 232, 0.64);
    cursor: pointer;
  }

  .rightmenu-item {
    /* display: flex; */
    align-items: center;
    text-align: center;
    min-width: max-content;
    border-radius: 10px ;
    font-size: 18px;
    font-weight: 600;
    font-family:Inter, sans-serif;
    /* cursor: pointer; */
    color: rgb(0, 0, 0);
  }
  .top-item {
    /* display: flex; */
    align-items: center;
    text-align: center;
    min-width: max-content;
    border-radius: 10px ;
    font-size: 18px;
    font-weight: 600;
    font-family:Inter, sans-serif;
  
    color: rgb(0, 0, 0);
  }


  @media screen and (max-width:1550px) {
    .music {
      display: none;
    }
  }
  @media screen and (max-width:950px) {
    .top{
      display: none;
    }

  }

</style>