<script>
  import { Posts } from "../posts.js";
  let elem = ""
  let elemImg = ""
  let elemVis = 0
  let elemText = ""
  Posts.forEach(el => {if(el.mark > elemVis){elemVis = el.mark; elem = el.title; elemImg = el.img; elemText = el.text }})

</script>

<div class="main-textarea">

  <div class="imgarea">
    <img class="cover" src={elemImg} alt="">
  </div>
  <div class="textarea">
    <h2>
      {elem}
    </h2> 
    <p>
      {elemText}
    </p>
  </div>
  
</div>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap');
  h2 {
    font-size: 16px;
    width: 200px;
    font-weight: 600;
    font-family:Inter, sans-serif;
    text-align: left;
    line-height: 1.3;
  }
  p {
    font-size: 12px;
    width: 200px;
    font-weight: 300;
    font-family:Inter, sans-serif;
    text-align: left;
    line-height: 1.4;
  }
  .textarea {
    display: flex;
    flex-direction: column;
    gap: 10px;
  }
  .main-textarea{
    justify-content: center;
    /* align-items: center; */
    display: flex;
    flex-direction: row;
    gap: 20px;
    cursor: pointer;
    /* position: relative; */
  }
  .cover {
    /* max-height: 100%; */
    display: block;
    
    /* max-width:100%; */
    object-fit: cover;
    margin: 0 auto;
    /* padding: 10px 10px 10px 10px; */
    border-radius: 10px;
    width: 100px;
    height: 100px;
  }
  .imgarea {
    /* position: absolute; */
    right: 0;
    top: 0;
    /* flex-basis: 35%; */
    /* position: relative; */
    height: 100px;
    width: 100px;
  }
  @media screen and (max-width:1550px) {
    .main-textarea{
      justify-content: center;

      display: flex;
      flex-direction: column;

    }
  }
  @media screen and (max-width:1000px) {
    .main-textarea{
      justify-content: center;

      display: flex;
      flex-direction: column;

    }
    h2 {
    width: 150px;
    }
    p {
      width: 150px;
    }
  }

</style>
