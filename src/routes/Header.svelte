<script>
  import {clickOutside} from './clickOutside.js';

  let visible = false;

  function toggleVissible() {
    visible = !visible      
  }
  function handleClickOutside(event) {
		if (visible) {
      visible = !visible
    }
	}
</script>

<div class="header">
  <div class="header-logo">
    
    <img class="imgarea" src="https://sun3-17.userapi.com/s/v1/if2/8mCAZiE4o221fU4x_bQwjuo7s5F8ws7K_OVwkW81JtWBnTyDbdomPX3Wwt6z9MbLjP1ZEcsuq2dmMvEA1knRqKoA.jpg?size=400x400&quality=96&crop=306,553,492,492&ava=1" alt="">
    <h1>PRO-Motivation</h1>
  </div>
  
  
  <div class="header-middle">
    <div class="search-div">
      <input type="search" placeholder="Поиск" class="search">
      <button class="search-button">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
          <path stroke-linecap="round" stroke-linejoin="round" d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
        </svg>
        
      </button>
    </div>
    <button class="search-button-mibile" on:click={toggleVissible}>
      <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
        <path stroke-linecap="round" stroke-linejoin="round" d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
      </svg> 
    </button>
    <button class="search-button-mibile-close" >
      <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
        <path stroke-linecap="round" stroke-linejoin="round" d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
      </svg> 
    </button>
    <div class="button-post">
      <button class="button">
        <svg  xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 svg-left-post">
          <path stroke-linecap="round" stroke-linejoin="round" d="M16.862 4.487l1.687-1.688a1.875 1.875 0 112.652 2.652L10.582 16.07a4.5 4.5 0 01-1.897 1.13L6 18l.8-2.685a4.5 4.5 0 011.13-1.897l8.932-8.931zm0 0L19.5 7.125M18 14v4.75A2.25 2.25 0 0115.75 21H5.25A2.25 2.25 0 013 18.75V8.25A2.25 2.25 0 015.25 6H10" />
        </svg>
        
        <span class="text-post">Добавить пост</span>
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 svg-right">
          <path stroke-linecap="round" stroke-linejoin="round" d="M12 4.5v15m7.5-7.5h-15" />
        </svg>
        
      </button>
    </div>
  </div>

  <div class="button-div enter">
    <button class="button">
      <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 svg-left">
        <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 6a3.75 3.75 0 11-7.5 0 3.75 3.75 0 017.5 0zM4.501 20.118a7.5 7.5 0 0114.998 0A17.933 17.933 0 0112 21.75c-2.676 0-5.216-.584-7.499-1.632z" />
      </svg>
      
      <span class="text">Войти</span>
    </button>
  </div>
  
</div>
{#if visible}
  <div class="mobile-search">
    <div class="search-div2" use:clickOutside on:click_outside={handleClickOutside}>
      <input type="search" placeholder="Поиск" class="search">
      <button class="search-button">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
          <path stroke-linecap="round" stroke-linejoin="round" d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
        </svg>
        
      </button>
    </div>
  </div>
{/if}
<div class="hamburger">
  <input id="menu__toggle" type="checkbox" />
  <label class="menu__btn" for="menu__toggle">
    <span></span>
  </label>

  <nuv class="leftmenu menu__box">
    <ul class="leftmenu-items">
      <ol class="leftmenu-item">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
          <path stroke-linecap="round" stroke-linejoin="round" d="M20.25 14.15v4.25c0 1.094-.787 2.036-1.872 2.18-2.087.277-4.216.42-6.378.42s-4.291-.143-6.378-.42c-1.085-.144-1.872-1.086-1.872-2.18v-4.25m16.5 0a2.18 2.18 0 00.75-1.661V8.706c0-1.081-.768-2.015-1.837-2.175a48.114 48.114 0 00-3.413-.387m4.5 8.006c-.194.165-.42.295-.673.38A23.978 23.978 0 0112 15.75c-2.648 0-5.195-.429-7.577-1.22a2.016 2.016 0 01-.673-.38m0 0A2.18 2.18 0 013 12.489V8.706c0-1.081.768-2.015 1.837-2.175a48.111 48.111 0 013.413-.387m7.5 0V5.25A2.25 2.25 0 0013.5 3h-3a2.25 2.25 0 00-2.25 2.25v.894m7.5 0a48.667 48.667 0 00-7.5 0M12 12.75h.008v.008H12v-.008z" />
        </svg>
        
        <span class="Sp">Бизнес</span>
      </ol>
      <ol class="leftmenu-item">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
          <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 21h19.5m-18-18v18m10.5-18v18m6-13.5V21M6.75 6.75h.75m-.75 3h.75m-.75 3h.75m3-6h.75m-.75 3h.75m-.75 3h.75M6.75 21v-3.375c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125V21M3 3h12m-.75 4.5H21m-3.75 3.75h.008v.008h-.008v-.008zm0 3h.008v.008h-.008v-.008zm0 3h.008v.008h-.008v-.008z" />
        </svg>
        
        <span class="Sp">Карьерный рост</span>
      </ol>
      <ol class="leftmenu-item"> 
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
          <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 18.75a60.07 60.07 0 0115.797 2.101c.727.198 1.453-.342 1.453-1.096V18.75M3.75 4.5v.75A.75.75 0 013 6h-.75m0 0v-.375c0-.621.504-1.125 1.125-1.125H20.25M2.25 6v9m18-10.5v.75c0 .414.336.75.75.75h.75m-1.5-1.5h.375c.621 0 1.125.504 1.125 1.125v9.75c0 .621-.504 1.125-1.125 1.125h-.375m1.5-1.5H21a.75.75 0 00-.75.75v.75m0 0H3.75m0 0h-.375a1.125 1.125 0 01-1.125-1.125V15m1.5 1.5v-.75A.75.75 0 003 15h-.75M15 10.5a3 3 0 11-6 0 3 3 0 016 0zm3 0h.008v.008H18V10.5zm-12 0h.008v.008H6V10.5z" />
        </svg>
           
        <span class="Sp">Финансы</span>
      </ol>
      <ol class="leftmenu-item">
        <svg width="24px" height="24px" fill="none" viewBox="0 0 32 32" version="1.1" stroke="currentColor" xmlns="http://www.w3.org/2000/svg">
          <title>medal</title>
          <path d="M15.999 13.531c-4.543 0-8.227 3.684-8.227 8.227s3.684 8.227 8.227 8.227c4.544 0 8.227-3.684 8.227-8.227s-3.683-8.227-8.227-8.227zM15.999 28.783c-3.844 0-6.961-3.117-6.961-6.963 0-3.844 3.117-6.96 6.961-6.96 3.846 0 6.961 3.116 6.961 6.96 0 3.846-3.115 6.963-6.961 6.963zM20.136 6.95l2.824-4.935h-13.922l2.867 4.935h8.231zM21.613 15.351l5.042-8.298-3.381-4.894-6.35 11.165c2.786 0.233 4.689 2.027 4.689 2.027zM15.053 13.262l-6.328-11.103-3.38 4.894 4.894 8.444c-0.001 0 1.776-1.832 4.814-2.235zM14.868 19.924c-0.383 0.299-0.736 0.5-1.062 0.607v1.131c0.619-0.203 1.157-0.518 1.613-0.945v4.711h1.25v-6.549h-1.014c-0.142 0.396-0.404 0.746-0.787 1.045z"></path>
          </svg>
        <span class="Sp">Спорт</span>
      </ol>
      <ol class="leftmenu-item">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
          <path stroke-linecap="round" stroke-linejoin="round" d="M4.26 10.147a60.436 60.436 0 00-.491 6.347A48.627 48.627 0 0112 20.904a48.627 48.627 0 018.232-4.41 60.46 60.46 0 00-.491-6.347m-15.482 0a50.57 50.57 0 00-2.658-.813A59.905 59.905 0 0112 3.493a59.902 59.902 0 0110.399 5.84c-.896.248-1.783.52-2.658.814m-15.482 0A50.697 50.697 0 0112 13.489a50.702 50.702 0 017.74-3.342M6.75 15a.75.75 0 100-1.5.75.75 0 000 1.5zm0 0v-3.675A55.378 55.378 0 0112 8.443m-7.007 11.55A5.981 5.981 0 006.75 15.75v-1.5" />
        </svg>
        
        <span class="Sp">Учёба</span>
      </ol>
      <ol class="leftmenu-item">
        <svg fill="#000000" height="24px" width="24px" version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" 
            viewBox="0 0 491.52 491.52" xml:space="preserve">
          <g>
            <g>
              <path d="M410.905,192.2C409.454,85.97,321.715,0,214.065,0C105.52,0,17.21,87.425,17.26,193.89
                c-0.27,2.785-6.06,68.895,41.085,136.085c20.27,28.895,33.38,56.535,40.085,84.5c4.55,18.955,7.85,51.355,7.85,77.045h20.48
                c0-27.095-3.54-61.505-8.41-81.825c-7.32-30.515-21.46-60.44-43.24-91.48C32.495,257.48,37.59,196.455,37.69,194.88
                c0-96.165,79.12-174.4,176.375-174.4s176.38,78.235,176.38,174.4v2.645l49.415,89.195h-44.06v92.16h-81.92v112.64h20.48v-92.16
                h81.92V307.2h58.34L410.905,192.2z"/>
            </g>
          </g>
          <g>
            <g>
              <path d="M354.84,220.6v-52.08l-33.435-5.57c-2.37-8.245-5.67-16.185-9.86-23.735l19.72-27.61l-36.825-36.83L266.83,94.5
                c-7.55-4.19-15.49-7.49-23.735-9.86L237.52,51.2h-52.075l-5.575,33.44c-8.245,2.37-16.185,5.67-23.735,9.86l-27.61-19.725
                L91.7,111.605l19.72,27.61c-4.19,7.55-7.49,15.49-9.86,23.73l-33.44,5.575v52.08l33.44,5.575c2.37,8.24,5.67,16.18,9.86,23.73
                l-19.72,27.61l36.825,36.83l27.61-19.725c7.55,4.19,15.49,7.49,23.735,9.86l5.575,33.44h52.075l5.575-33.44
                c8.245-2.37,16.185-5.67,23.735-9.86l27.61,19.725l36.825-36.83l-19.72-27.61c4.19-7.55,7.49-15.49,9.86-23.735L354.84,220.6z
                M304.625,208.205l-1.495,6.755c-2.345,10.6-6.53,20.68-12.44,29.96l-3.715,5.83l17.54,24.555l-12.285,12.29l-24.565-17.545
                l-5.83,3.715c-9.27,5.91-19.35,10.095-29.96,12.45l-6.75,1.495l-4.955,29.73h-17.375l-4.955-29.73l-6.75-1.495
                c-10.61-2.355-20.69-6.54-29.96-12.45l-5.83-3.715l-24.565,17.545l-12.285-12.29l17.54-24.555l-3.715-5.83
                c-5.91-9.28-10.095-19.36-12.44-29.96l-1.495-6.755l-29.74-4.955v-17.38l29.74-4.955l1.495-6.755
                c2.345-10.6,6.53-20.68,12.44-29.96l3.715-5.83l-17.54-24.555l12.285-12.29l24.565,17.545l5.83-3.715
                c9.27-5.91,19.35-10.095,29.96-12.45l6.75-1.495l4.955-29.73h17.375l4.955,29.73l6.75,1.495c10.61,2.355,20.69,6.54,29.96,12.45
                l5.83,3.715l24.565-17.545l12.285,12.29l-17.54,24.555l3.715,5.83c5.91,9.28,10.095,19.36,12.44,29.96l1.495,6.755l29.735,4.955
                v17.38L304.625,208.205z"/>
            </g>
          </g>
          <g>
            <g>
              <path d="M211.479,132.23c-34.37,0-62.33,27.96-62.33,62.33s27.96,62.33,62.33,62.33c34.37,0,62.335-27.96,62.335-62.33
                S245.85,132.23,211.479,132.23z M211.479,236.41c-23.075,0-41.85-18.775-41.85-41.85s18.775-41.85,41.85-41.85
                c23.08,0,41.855,18.775,41.855,41.85S234.56,236.41,211.479,236.41z"/>
            </g>
          </g>
        </svg>
        
        <span class="Sp">Саморазвитие</span>
      </ol>
    </ul>
    <div class="leftmenu-items2">
      <p>О нас</p>
      <p>
        <span class="sp">Мы в Telegram</span> 
        <svg width="24px" height="24px" viewBox="0 0 256 256" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" preserveAspectRatio="xMidYMid">
          <g>
              <path d="M128,0 C57.307,0 0,57.307 0,128 L0,128 C0,198.693 57.307,256 128,256 L128,256 C198.693,256 256,198.693 256,128 L256,128 C256,57.307 198.693,0 128,0 L128,0 Z" fill="#40B3E0">
      
      </path>
              <path d="M190.2826,73.6308 L167.4206,188.8978 C167.4206,188.8978 164.2236,196.8918 155.4306,193.0548 L102.6726,152.6068 L83.4886,143.3348 L51.1946,132.4628 C51.1946,132.4628 46.2386,130.7048 45.7586,126.8678 C45.2796,123.0308 51.3546,120.9528 51.3546,120.9528 L179.7306,70.5928 C179.7306,70.5928 190.2826,65.9568 190.2826,73.6308" fill="#FFFFFF">
      
      </path>
              <path d="M98.6178,187.6035 C98.6178,187.6035 97.0778,187.4595 95.1588,181.3835 C93.2408,175.3085 83.4888,143.3345 83.4888,143.3345 L161.0258,94.0945 C161.0258,94.0945 165.5028,91.3765 165.3428,94.0945 C165.3428,94.0945 166.1418,94.5735 163.7438,96.8115 C161.3458,99.0505 102.8328,151.6475 102.8328,151.6475" fill="#D2E5F1">
      
      </path>
              <path d="M122.9015,168.1154 L102.0335,187.1414 C102.0335,187.1414 100.4025,188.3794 98.6175,187.6034 L102.6135,152.2624" fill="#B5CFE4">
      
      </path>
          </g>
      </svg>
      </p>
      <p >
        <span class="sp">Мы в Vkontakte</span>
        <svg width="24px" height="24px" viewBox="0 0 202 202" id="VK_Logo" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
  
          <style>.st0{clip-path:url(#SVGID_2_);fill:#5181b8}.st1{fill-rule:evenodd;clip-rule:evenodd;fill:#fff}</style>
          
          <g id="Base">
          
          <defs>
          
          <path id="SVGID_1_" d="M71.6 5h58.9C184.3 5 197 17.8 197 71.6v58.9c0 53.8-12.8 66.5-66.6 66.5H71.5C17.7 197 5 184.2 5 130.4V71.5C5 17.8 17.8 5 71.6 5z"/>
          
          </defs>
          
          <use xlink:href="#SVGID_1_" overflow="visible" fill-rule="evenodd" clip-rule="evenodd" fill="#5181b8"/>
          
          <clipPath id="SVGID_2_">
          
          <use xlink:href="#SVGID_1_" overflow="visible"/>
          
          </clipPath>
          
          <path class="st0" d="M0 0h202v202H0z"/>
          
          </g>
          
          <path id="Logo" class="st1" d="M162.2 71.1c.9-3 0-5.1-4.2-5.1h-14c-3.6 0-5.2 1.9-6.1 4 0 0-7.1 17.4-17.2 28.6-3.3 3.3-4.7 4.3-6.5 4.3-.9 0-2.2-1-2.2-4V71.1c0-3.6-1-5.1-4-5.1H86c-2.2 0-3.6 1.7-3.6 3.2 0 3.4 5 4.2 5.6 13.6v20.6c0 4.5-.8 5.3-2.6 5.3-4.7 0-16.3-17.4-23.1-37.4-1.4-3.7-2.7-5.3-6.3-5.3H42c-4 0-4.8 1.9-4.8 4 0 3.7 4.7 22.1 22.1 46.4C70.9 133 87.2 142 102 142c8.9 0 10-2 10-5.4V124c0-4 .8-4.8 3.7-4.8 2.1 0 5.6 1 13.9 9 9.5 9.5 11.1 13.8 16.4 13.8h14c4 0 6-2 4.8-5.9-1.3-3.9-5.8-9.6-11.8-16.4-3.3-3.9-8.2-8-9.6-10.1-2.1-2.7-1.5-3.9 0-6.2 0-.1 17.1-24.1 18.8-32.3z"/>
          
          </svg>
      </p>
    </div>
  
  </nuv>
</div>




<style>
    @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap');
  .leftmenu {
    /* background-color: rgb(242, 242, 242); */
    /* width: 500; */
    height: 100%;
    min-height: 50%;
    border-radius: 0 10px 10px 0;
    margin: 100px 0 0 0 ;
    padding: 40px 40px 40px 40px;
    display: flex;
    position: fixed;
    flex-direction: column;
    gap: 40px; 
  }
  .leftmenu-items {
    border-radius: 0 0 10px 0;
    margin: 0 ;
    margin-top: 50px;
    display: flex;
    flex-direction: column;
    gap: 30px; 
  }
  .leftmenu-items2 {
    bottom: 20px;
    position: absolute;
    margin-top: auto;
    display: flex;
    flex-direction: column;
    gap: 20px; 
  }
  .leftmenu-item {
    display: flex;
    align-items: center;
    min-width: max-content;
    border-radius: 10px ;
    font-size: 18px;
    font-weight: 600;
    font-family:Inter, sans-serif;
    cursor: pointer;
    color: rgb(0, 0, 0);
  }
  .leftmenu-item:hover {

    color: rgb(35, 70, 2);

  }
  p {
    font-family:Inter, sans-serif;
    cursor: pointer;
    font-size: 14px;
    font-weight: 400;
    display: flex;
    align-items: center;
  }

  p:hover {
    font-family:Inter, sans-serif;
    cursor: pointer;
    font-size: 14px;
    font-weight: 400;
    color: rgb(35, 70, 2);
  }

  .Sp {
    margin-left: 10px;
  }
  .sp {
    margin-right: 10px;
  }
  
  #menu__toggle {
    position: fixed;
    opacity: 0;
  }
  #menu__toggle:checked + .menu__btn > span {
    transform: rotate(45deg);
  }
  #menu__toggle:checked + .menu__btn > span::before {
    top: 0;
    transform: rotate(0deg);
  }
  #menu__toggle:checked + .menu__btn > span::after {
    top: 0;
    transform: rotate(90deg);
  }
  #menu__toggle:checked ~ .menu__box {
    left: 0 !important;
  }
  .menu__btn {
    position: fixed;
    top: 45px;
    left: 35px;
    width: 26px;
    height: 26px;
    cursor: pointer;
    z-index: 1;
  }
  .menu__btn > span,
  .menu__btn > span::before,
  .menu__btn > span::after {
    display: block;
    position: absolute;
    width: 100%;
    height: 2px;
    background-color: #616161;
    transition-duration: .25s;
  }
  .menu__btn > span::before {
    content: '';
    top: -8px;
  }
  .menu__btn > span::after {
    content: '';
    top: 8px;
  }
  .menu__box {
    display: block;
    position: fixed;
    top: 0;
    left: -100%;
    width: 250px;
    height: 100%;
    margin: 0;
    /* padding: 80px 0; */
    list-style: none;
    background-color: #ECEFF1;
    box-shadow: 2px 2px 6px rgba(0, 0, 0, .4);
    transition-duration: .25s;
  }
  .menu__item {
    display: block;
    padding: 12px 24px;
    color: #333;
    font-family: 'Roboto', sans-serif;
    font-size: 20px;
    font-weight: 600;
    text-decoration: none;
    transition-duration: .25s;
  }
  .menu__item:hover {
    background-color: #CFD8DC;
  }
  .header {
    /* background-color: rgba(239, 239, 239, 0.846); */
    backdrop-filter: blur(10px);
    margin-right: auto;
    padding-top: 20px;
    width: 100%;
    padding-bottom: 20px;
    position: fixed;
  }
  .search-button-mibile{
    display: none;
  }
  .search-button-mibile-close{
    display: none;
  }
  .mobile-search{
    display: none;
  }
  .header-middle {
    /* background-color: rgb(206, 219, 219); */
    max-width: 840px;
    min-width: 0px;
    border-radius: 10px;
    margin: 0 auto;
    /* right: 0; */
    /* padding: 20px 0 20px 0 ; */
    display: flex;
    /* flex-direction: column; */
    justify-content: space-between;
    width: 100%;
    align-items: center;
    gap: 20px;
  }
  .button-div {
    background-color: rgb(222, 239, 239);
    position: relative;
    border-radius: 10px;
    /* margin: 0 auto; */
    /* padding: 15px; */
    margin-left: auto;
    display: flex;
    /* flex-direction: row; */
    gap: 20px;
    padding: 5px;
  }
  .button-post {
    background-color: rgb(222, 239, 239);
    position: relative;
    border-radius: 10px;
    /* margin: 0 auto; */
    /* padding: 15px; */
    margin-left: auto;
    display: flex;
    /* flex-direction: row; */
    gap: 20px;
    padding: 5px;
  }
  .button {
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
  .button:hover {
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
  .text {
    padding: 10px;
  }
  .text-post {
    padding: 10px;
  }
  .imgarea {
    
    /* position: absolute; */
    /* right: 0; */
    /* top: 0; */
    /* flex-basis: 35%; */
    /* position: relative; */
    border-radius: 100%;
    height: 50px;
    width: 50px;
  }
  .header-logo {
    display: flex;
    position: absolute;
    align-items: center;
    padding-left: 40px;
    height: 50px;
    /* margin: 0 50px 0 0; */
  }
  h1 {
    margin-left: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
    min-width: max-content;
    font-size: 25px;
    font-weight: 600;
    font-family:Inter, sans-serif;
    cursor: pointer;
  }
  .svg-left {
    margin-left:  10px;
  }
  .svg-left-post {
    margin-left:  10px;
  }
  .svg-right {
    margin-right:  10px;
  }
  .search {
    border-radius: 10px;
    height: 48px;
    width: 300px;
    font-family:Inter, sans-serif;
    background-color: rgb(222, 239, 239);
    border: 0;
    color: black;
  }
  .search-div {
    height: 50px;
    position: relative;
  }
  .search-div2 {
    height: 50px;
    width: 100%;
    display: none;
  }
  .search-button {
    position: absolute;
    right: 10px;
    padding-top: 13px;


  }
  .search-button:hover {
    cursor: pointer;
    transform:scale(1.05);
    transition: 0.1s linear;
  }
  .enter {
    position: absolute;
    display: flex;
    align-items: center;
    right: 0;
    margin-right: 40px;
    top: 0;
    margin-top: 20px;
  }
  .hamburger {
    display: none;
  }
  @media screen and (max-width:1720px) {
    .header-middle {
      /* background-color: rgb(206, 219, 219); */
      max-width: 840px;
      min-width: 0px;
      border-radius: 10px;
      margin: 0 440px auto auto;
      /* right: 0; */
      /* padding: 20px 0 20px 0 ; */
      display: flex;
      /* flex-direction: column; */
      justify-content: space-between;
      width: 100%;
      align-items: center;
      gap: 20px;
    }
  }
  @media screen and (max-width:1600px) {
    h1 {
      margin-left: 15px;
      display: flex;
      justify-content: center;
      align-items: center;
      min-width: max-content;
      font-size: 18px;
      font-weight: 600;
      font-family:Inter, sans-serif;
      cursor: pointer;
   }
  }
  @media screen and (max-width:1550px) {
    .header-middle {
      /* background-color: rgb(206, 219, 219); */
      max-width: 840px;
      margin: 0 310px auto auto;
    }
  }
  @media screen and (max-width:1435px) {
    .header-middle {
        /* background-color: rgb(206, 219, 219); */
        max-width: 800px;
        margin: 0 310px auto auto;
      }
  }
  @media screen and (max-width:1394px) {
    .header-middle {
        /* background-color: rgb(206, 219, 219); */
        max-width: 760px;
        margin: 0 310px auto auto;
      }
  }
  @media screen and (max-width:1340px) {
    .header-logo {
      display: flex;
      position: absolute;
      align-items: center;
      padding-left: 20px;
      height: 50px;
      /* margin: 0 50px 0 0; */
    }
    h1 {
      margin-left: 10px;
      font-size: 18px;
    }
    .leftmenu-item {
      display: flex;
      align-items: center;
      min-width: max-content;
      border-radius: 10px ;
      font-size: 14px;
      font-weight: 600;
      font-family:Inter, sans-serif;
      cursor: pointer;
      color: rgb(0, 0, 0);
    }
    p {
      font-family:Inter, sans-serif;
      cursor: pointer;
      font-size: 12px;
      font-weight: 400;
      display: flex;
      align-items: center;
    }

    p:hover {
      font-family:Inter, sans-serif;
      cursor: pointer;
      font-size: 12px;
      font-weight: 400;
      color: rgb(35, 70, 2);
    }
  }
  @media screen and (max-width:1310px) {
    .header-middle {
        /* background-color: rgb(206, 219, 219); */
        max-width: 720px;
        margin: 0 310px auto auto;

      }
  }
  @media screen and (max-width:1280px) {
    .header-middle {
        /* background-color: rgb(206, 219, 219); */
        max-width: 680px;
        min-width: 0px;
        border-radius: 10px;
        margin: 0 310px auto auto;
        /* right: 0; */
        /* padding: 20px 0 20px 0 ; */
        display: flex;
        /* flex-direction: column; */
        justify-content: space-between;
        width: 100%;
        align-items: center;
        gap: 20px;
      }
  }
  @media screen and (max-width:1230px) {
    h1{
      font-size: 16px;
    }
  }
  @media screen and (max-width:1200px) {
    h1 {
      display: none;
    }
    .header-logo {
      display: flex;
      position: absolute;
      align-items: center;
      margin-left: 70px;
      height: 50px;
      /* margin: 0 50px 0 0; */
    }
    .imgarea {
      border-radius: 100%;
      height: 50px;
      width: 50px;
    }
    .hamburger {
      display: block;

    }
    .header-middle {
      /* background-color: rgb(206, 219, 219); */
      max-width: 440px;
    }

  }
  @media screen and (max-width:950px) {
    .header-middle {
      /* background-color: rgb(206, 219, 219); */
      max-width: 340px;
    }
    .svg-right {
      display: none;;
    }
    .svg-left-post {
      margin-right: 10px;
    }
    .text-post {
      display: none;
    }
    .button-post {
      height: 48px;
      width: 48px;
      margin-bottom: 2px;
    }

  }
  @media screen and (max-width:850px) {
    .search {
      width: 300px;
      /* margin-right: 20px; */
      /* right: 0; */
      
    }
    .header-middle {
      /* background-color: rgb(206, 219, 219); */
      max-width: 340px;
      gap: 10px;
    }
    .button-post {
      height: 48px;
      width: 48px;
      margin-bottom: 2px;
      /* margin-left: 0px; */
    }
    .header-middle {
      margin-right: 180px;
    }

  }
  @media screen and (max-width:700px) {
    .search {
      width: 180px;
    }

    .header-middle {
      /* background-color: rgb(206, 219, 219); */
      max-width: 250px;
      gap: 10px;
    }
    .button-post {
      height: 48px;
      width: 48px;
      margin-bottom: 2px;
      /* margin-left: 0px; */
    }
    .header-middle {
      margin-right: 180px;
    }

  }
  @media screen and (max-width:600px) {
    .search-div {
      display: none;
    }
    .mobile-search {
      backdrop-filter: blur(10px);
      display: block;
      padding-bottom: 20px;
      width: 100%;
      align-content: center;
      align-items: center;
      position: fixed;
      padding-top: 90px;
    }
    .search-div2 {
      display: block;
      /* position: fixed; */
      /* flex-direction: column; */
      /* margin-top: 90px; */
      width: 70%;
      margin-left: auto;
      margin-right: auto;
      position: relative;
      

    }
    .search{
      height: 100%;
      width: 100%;
    }
    .search-button {
    position: absolute;
    }
    .search-button-mibile{
      display: block;
      background-color: rgb(222, 239, 239);
      padding: 12px;
      margin-bottom: 2px;
      border-radius: 10px;

    }
    .header-middle {
      max-width: 120px;
      margin-right: 100px;
    }
    .button-post {
      display: none;
    }


  }


</style>