<script>
  export let ArtTitle = ""
  export let ArtText =""
  export let ArtImg =""

</script>

<div class="main-textarea">
  <div class="textarea">
      <h2>
        {ArtTitle}
      </h2>
      <p>
        {ArtText}
      </p> 
  </div>
  <div class="imgarea">
    <img class="cover" src={ArtImg} alt="">
  </div>
  
</div>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap');
  h2 {
    font-size: 28px;
    font-weight: 600;
    font-family:Inter, sans-serif;
    line-height: 1.2;
  }
  p {
    font-size: 19px;
    font-weight: 400;
    font-family:Inter, sans-serif;
    line-height: 1.2;
  }
  .textarea {
    display: flex;
    flex-direction: column;
    gap: 20px;
    flex-basis: 80%;
  }
  .main-textarea{
    display: flex;
    flex-direction: column;
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
    width: 100%;
    height: 350px;
  }
  .imgarea {
    /* position: absolute; */

    /* right: 0; */
    /* top: 0; */
    /* flex-basis: 35%; */
    /* position: relative; */
    height: 350px;
    width: 100%;
  }
  @media screen and (max-width:1050px) {
    .textarea {
      flex-basis: 80%;
    }
    h2 {
      font-size: 26px;
    }
    p {
      font-size: 16px;
    }
    .imgarea {
      height: 300px;
      width: 100%;
    }
    .cover {
    /* max-height: 100%; */
      display: block;
      
      /* max-width:100%; */
      object-fit: cover;
      margin: 0 auto;
      /* padding: 10px 10px 10px 10px; */
      border-radius: 10px;
      width: 100%;
      height: 300px;
    }

  }
  @media screen and (max-width:650px) {
    .textarea {
      display: flex;
      flex-direction: column;
      gap: 20px;
      flex-basis: 80%;
    }
    h2 {
      font-size: 24px;
      font-weight: 600;
      font-family:Inter, sans-serif;
      line-height: 1.2;
    }
    p {
      font-size: 15px;
      font-weight: 400;
      font-family:Inter, sans-serif;
      line-height: 1.2;
    }

  }
  @media screen and (max-width:450px) {
    .imgarea {
      height: 250px;
    }
    .cover {
      height: 250px;
    }
  }
</style>
