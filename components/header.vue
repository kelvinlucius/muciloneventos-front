<template>
      <nav id="sidebar" class="sidebar-wrapper ">
        <div class="soNoMobile">
            <div class="d-flex justify-content-end">Logo</div>
        </div>
        <div class="soNoDescktop">
            <div class="d-flex bd-highlight mb-3  wrapper">
                <div class="mr-auto p-2 bd-highlight">Logo</div>
                <div class="p-2 bd-highlight">Sobre nos</div>
                <div class="p-2 bd-highlight">Nosso trabalho</div>
            </div>
        </div>
    </nav>
    <input id="check" type="checkbox" />
    <label for="check" id="icone">
      <div id="container-hamburguer" class="menu">
        <span id="hamburguer" class="hamburguer"></span>
      </div>
    </label>
    <div id="barra" class="barra">
        <div class="itensBarra">
            <div class="itemBarra">
                <p>Sobre nos</p>
            </div>
            <div class="itemBarra">
                <p>Sobre nos</p>
            </div>
        </div>
    </div>

</template>

<script>
    export default{
      setup(){
        //window.addEventListener("scroll", function(){
        //  alert('teste');
        //});


        return{

        }
      }
    }

</script>
  


 
  <style>
html {
    margin: 0;
    padding: 0;
}

body {
    width: 100%;
    margin: 0;
    padding: 0;
}

.sidebar-color {
    background: #6CC28F !important;
}

.sidebar-wrapper {
    background: rgba(0, 0, 255, 0.212);
    position: fixed;
    width: 100%;
}

.wrapper {
    width: 100%;
    max-width: 1200px;
    margin: auto;
}

input {
    display: none;
}

.itemBarra {
    display: none;
}

.soNoMobile {
    display: none;
}

@media screen and (max-width: 770px) {
    .soNoMobile {
        display: block;
    }
    .soNoDescktop {
        display: none;
    }
    .itensBarra {
        margin-top: 80px;
        position: fixed;
    }
    .itemBarra {
        display: block;
        color: white;
    }
    .menu {
        background: white;
        border-radius: 50%;
        width: 60px;
        height: 60px;
        position: fixed;
        top: 10px;
        left: 25px;
        z-index: 1;
    }
    .hamburguer {
        position: relative;
        display: block;
        background: #000;
        width: 30px;
        height: 2px;
        top: 28px;
        left: 15px;
        transition: 0.5s ease-in-out;
    }
    .hamburguer:before,
    .hamburguer:after {
        background: #000;
        content: '';
        display: block;
        width: 100%;
        height: 100%;
        position: absolute;
        transition: 0.5s ease-in-out;
    }
    .hamburguer:before {
        top: -10px;
    }
    .hamburguer:after {
        bottom: -10px;
    }
    .hamburguer-mover:before {
        top: -10px;
    }
    .hamburguer-mover:after {
        bottom: -10px;
    }
    .hamburguer-mover {
        transform: rotate(45deg);
    }
    .hamburguer-mover:before {
        transform: rotate(90deg);
        top: 0;
    }
    .hamburguer-mover:after {
        transform: rotate(90deg);
        bottom: 0;
    }
    /**  css menu latel mobile*/
    .barra {
        background-color: #333;
        height: 100%;
        width: 300px;
        position: fixed;
        transition: all .2s linear;
        left: -300px;
        top: 0;
    }
    /**  animaÃ§ÃĢo menu latel mobile*/
    .barra-aberta {
        transform: translateX(300px);
    }
    .sidebar-wrapper {
        height: 80px;
    }
}

  </style>