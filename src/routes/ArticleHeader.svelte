

<div class="Header">
  <div class="Autor">
    <img class="svg" src="https://2ds.ru/posts/example-golang/poster.jpg" alt="">
    <div class="Name">Павел Баев</div>
  </div>
  <div class="Views">
    <svg width="24px" height="24px" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="svg">
      <path fill-rule="evenodd" clip-rule="evenodd" d="M22 12.0002C20.2531 15.5764 15.8775 19 11.9998 19C8.12201 19 3.74646 15.5764 2 11.9998" stroke="#000000" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
      <path fill-rule="evenodd" clip-rule="evenodd" d="M22 12.0002C20.2531 8.42398 15.8782 5 12.0005 5C8.1227 5 3.74646 8.42314 2 11.9998" stroke="#000000" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
      <path d="M15 12C15 13.6569 13.6569 15 12 15C10.3431 15 9 13.6569 9 12C9 10.3431 10.3431 9 12 9C13.6569 9 15 10.3431 15 12Z" stroke="#000000" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
      </svg>
    <div class="ViewsNum">2000</div>
  </div>
</div>



<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap');
  .Header {
    display: flex;
    flex-direction: row;
    gap: 40px;
    max-height: 24px;
  }
  .Autor {
    display: flex;
    flex-direction: row;
    gap: 5px;
    cursor: pointer;

  }
  .Autor .svg {
    /* display: inline; */
    height: 24px;
    width: 24px;
    object-fit: cover;
    border-radius: 5px;
  }
  .Autor .Name{
    display: flex;
    /* vertical-align: middle; */
    align-items: center;
    align-content: center;
    justify-content: center;
 
    font-size: 16px;
    font-weight: 500;
    font-family:Inter, sans-serif
  }
  .Views {
    display: flex;
    flex-direction: row;
    gap: 5px;
    align-items: center;
    align-content: center;
    justify-content: center;
    
  }
  .Views .svg {
    /* display: flex; */
    height: 20px;
    width: 20px;
    object-fit:cover;
    align-items: center;
    align-content: center;
    border-radius: 5px;
    /* padding-top: 2px; */


  }
  .Views .ViewsNum{
    display: flex;
    /* vertical-align: middle; */
    align-items: center;
    align-content: center;
    justify-content: center;

    font-size: 16px;
    font-weight: 500;
    font-family:Inter, sans-serif
  }

</style>
