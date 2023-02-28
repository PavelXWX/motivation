<script>
  export let ArtTitle = ""
  export let ArtText =""

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
  
</div>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap');
  h2 {
    color: aliceblue;
    font-size: 28px;
    font-weight: 600;
    font-family:Inter, sans-serif;
    line-height: 1.2;
  }
  p {
    color: aliceblue;
    font-size: 19px;
    font-weight: 400;
    font-family:Inter, sans-serif;
    line-height: 1.2;
  }
  .textarea {
    display: flex;
    flex-direction: column;
    gap: 20px;
    flex-basis: 100%;
  }
  .main-textarea{
    display: flex;
    flex-direction: row;
    gap: 20px;
    cursor: pointer;
    /* position: relative; */
  }
  @media screen and (max-width:1050px) {
    h2 {
      font-size: 26px;
    }
    p {
      font-size: 16px;
    }

  }
  @media screen and (max-width:650px) {
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
</style>
