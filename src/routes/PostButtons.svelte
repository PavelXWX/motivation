<script>
  let active = {button1: false, button2: false, button3: false}
</script>

<div class="Modal">
  <button class="But" class:active="{active.button1}" on:click={() => {active.button1 = !active.button1; active.button2=false; active.button3=false}}>
    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
      <path stroke-linecap="round" stroke-linejoin="round" d="M15.59 14.37a6 6 0 01-5.84 7.38v-4.8m5.84-2.58a14.98 14.98 0 006.16-12.12A14.98 14.98 0 009.631 8.41m5.96 5.96a14.926 14.926 0 01-5.841 2.58m-.119-8.54a6 6 0 00-7.381 5.84h4.8m2.581-5.84a14.927 14.927 0 00-2.58 5.84m2.699 2.7c-.103.021-.207.041-.311.06a15.09 15.09 0 01-2.448-2.448 14.9 14.9 0 01.06-.312m-2.24 2.39a4.493 4.493 0 00-1.757 4.306 4.493 4.493 0 004.306-1.758M16.5 9a1.5 1.5 0 11-3 0 1.5 1.5 0 013 0z" />
    </svg>
    
    <span class="Te">
      Новое
    </span>
  </button>
  <button class="But" class:active="{active.button2}" on:click={() => {active.button2 = !active.button2; active.button1=false; active.button3=false}}>
    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
      <path stroke-linecap="round" stroke-linejoin="round" d="M15.362 5.214A8.252 8.252 0 0112 21 8.25 8.25 0 016.038 7.048 8.287 8.287 0 009 9.6a8.983 8.983 0 013.361-6.867 8.21 8.21 0 003 2.48z" />
      <path stroke-linecap="round" stroke-linejoin="round" d="M12 18a3.75 3.75 0 00.495-7.467 5.99 5.99 0 00-1.925 3.546 5.974 5.974 0 01-2.133-1A3.75 3.75 0 0012 18z" />
    </svg>
    
    <span class="Te">
      Популярное
    </span>
  </button>
  <button class="But" class:active="{active.button3}" on:click={() => {active.button3 = !active.button3; active.button2=false; active.button1=false}}>
    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
      <path stroke-linecap="round" stroke-linejoin="round" d="M10.34 15.84c-.688-.06-1.386-.09-2.09-.09H7.5a4.5 4.5 0 110-9h.75c.704 0 1.402-.03 2.09-.09m0 9.18c.253.962.584 1.892.985 2.783.247.55.06 1.21-.463 1.511l-.657.38c-.551.318-1.26.117-1.527-.461a20.845 20.845 0 01-1.44-4.282m3.102.069a18.03 18.03 0 01-.59-4.59c0-1.586.205-3.124.59-4.59m0 9.18a23.848 23.848 0 018.835 2.535M10.34 6.66a23.847 23.847 0 008.835-2.535m0 0A23.74 23.74 0 0018.795 3m.38 1.125a23.91 23.91 0 011.014 5.395m-1.014 8.855c-.118.38-.245.754-.38 1.125m.38-1.125a23.91 23.91 0 001.014-5.395m0-3.46c.495.413.811 1.035.811 1.73 0 .695-.316 1.317-.811 1.73m0-3.46a24.347 24.347 0 010 3.46" />
    </svg>
    
    <span class="Te">
      Интересное
    </span>
  </button>
</div>


<style>
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap');
  .Modal {
    background-color: rgb(222, 239, 239);
    /* position: relative; */
    border-radius: 10px;
    margin-right: auto;
    /* margin: 0 auto; */
    /* padding: 15px; */
    display: flex;
    flex-direction: row;
    gap: 20px;
    padding: 5px;
  }
  .But {
    display: flex;
    justify-content: center;
    align-items: center;
    min-width: max-content;
    border-radius: 10px ;
    /* width: 250px; */
    /* padding: 0 20px 0 20px; */
    /* height: 45px; */
    font-size: 18px;
    font-weight: 500;
    font-family:Inter, sans-serif;
    cursor: pointer;
    /* border-width: 2px; */
    /* border-color: rgb(0, 0, 0); */
    color: rgb(0, 0, 0);
  }
  .But:hover {
    display: flex;
    background-color: rgb(225, 225, 225);
    justify-content: center;
    align-items: center;
    min-width: max-content;
    border-radius: 10px ;
    /* width: 250px; */
    /* padding: 0 20px 0 20px; */
    /* height: 45px; */
    font-size: 18px;
    font-weight: 500;
    font-family:Inter, sans-serif;
    cursor: pointer;
    /* border-width: 2px; */
    /* border-color: rgb(0, 0, 0); */
    color: rgb(35, 70, 2);
  }
  .active {
    display: flex;
    background-color: rgb(225, 225, 225);
    justify-content: center;
    align-items: center;
    min-width: max-content;
    border-radius: 10px ;
    /* width: 250px; */
    /* padding: 0 20px 0 20px; */
    /* height: 45px; */
    font-size: 18px;
    font-weight: 500;
    font-family:Inter, sans-serif;
    cursor: pointer;
    /* border-width: 2px; */
    /* border-color: rgb(0, 0, 0); */
    color: rgb(35, 70, 2);
  }

  .Te {
    padding: 10px 10px 10px 10px;
    
  }
  svg {
    margin-left:  10px;
  }
  @media screen and (max-width:950px) {
    .Modal {

      margin: 0 auto;
    }

  }
  @media screen and (max-width:550px) {
    .But {
      font-size: 14px;
    }

  }
  @media screen and (max-width:500px) {
    .But {
      flex-direction: column;
      font-size: 14px;
    }
    .Modal {
      padding-top: 5px;
      gap: 7px;
    }
    svg {
      padding-top: 5px;
    }

  }
  



</style>