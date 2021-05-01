<template>
  <div id="app" class="lg:px-20 height">
    <router-view/>
  </div>
</template>

<style lang="scss">
$color-gray : #D3DCE6;
$color-black: #131313;
$eye-color: #575A65;
$border-radius:20px;

@font-face {
  src: url("./assets/Graphik-Font-Family/GraphikRegular.otf");
  font-family: Graphik;
}

#app {
  font-family: "Graphik";
  font-size: 16px;
  color: $color-gray;
  overflow: hidden;
}

.height {
  height: 100vh;
}

.bg-dark{
  background-color: $color-black;
}
.text-gray{
  color:$color-gray;
}

.rounded-custom{
  border-radius: $border-radius;
}

.col{
  padding: 0;
  width:499px;
}

.h-50{
  height:305px;
}
.bg-image{
  width: 364px;
  background-image: url('./assets/patricia-icon.png');
  background-repeat: no-repeat;
  background-position: left;
  background-size: cover;
  height: 100%;
}
.mx-4{
  margin:0 20px ;
}

.px-40-custom{
  padding: 0 70px;
}

.px-12-custom{
  padding: 25px 33px;
}
.h4{
  font-size: 32px;
}
.h5{
  font-size: 23px;
}

.card-text{
  font-size: 14px;
}

@media screen and (max-width: 600px){
  .col{
    padding: 0;
    width:399px;
    margin: 0 auto;
  }

  .h-50{
    height:245px;
  }

  .height {
    height: auto;
  }
  .px-2-custom{
    padding: 0 3px;
  }

  .rounded-custom{
    border-radius: 14px;
  }

}

@media screen and (max-width: 450px){
  .col{
    padding: 0;
    width:340px;
    margin: 0 auto;
  }

  .bg-image{
    width: 90%;
  }

  .bg-dark{
    overflow: hidden;
  }
  .h-50{
    height:35vh;
  }

  .h5,.h4{
    font-size: 16px;
  }

  #app {
    font-size: 12px;
  }

  .height {
    height: auto;
  }

  .rounded-custom{
    border-radius: 13px;
  }
}
</style>
