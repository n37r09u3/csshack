<template>
  <div class="home">

    <div class="arwes">
      <div class="border top"></div>
      <div class="border bottom"></div>
      <div class="border right"></div>
      <div class="border left"></div>
      <div class="corner top-left">

      </div>
      <div class="corner top-right">

      </div>
      <div class="corner bottom-left">

      </div>
      <div class="corner bottom-right">

      </div>
      <button class="button">按钮</button>

    </div>

  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  components: {
  }
}
</script>



<style lang="scss">


.arwes {
position: relative;
display: inline-block;


  .border{

    &.top{
      top: 0;
      width: 100%;
      border-width: 1px 0 0 0;
      opacity: 1;
      position: absolute;
      transition: all 250ms ease-in;
      border-style: solid;
      border-color: #4bf2f6;
      box-shadow: 0 0 4px rgba(75,242,246,0.65);
    }
    &.bottom{
      bottom: 0;
      width: 100%;
      border-width: 1px 0 0 0;
      opacity: 1;
      position: absolute;
      transition: all 250ms ease-in;
      border-style: solid;
      border-color: #4bf2f6;
      box-shadow: 0 0 4px rgba(75,242,246,0.65);
    }
    &.left{
      z-index: 1;
      opacity: 1;
      position: absolute;
      transition: all 250ms ease-in;
      border-style: solid;
      left: 0;
      height: 100%;
      border-width: 0 0 0 1px;
      border-color: #4bf2f6;
      box-shadow: 0 0 4px rgba(75,242,246,0.65);
    }
    &.right{
      z-index: 1;
      opacity: 1;
      position: absolute;
      transition: all 250ms ease-in;
      border-style: solid;
      right: 0;
      height: 100%;
      border-width: 0 0 0 1px;
      border-color: #4bf2f6;
      box-shadow: 0 0 4px rgba(75,242,246,0.65);
    }
  }
  .corner{
    &.top-left{
      z-index: 2;
      top: 0;
      width: 5px;
      height: 5px;
      border-width: 1px 0 0 1px;
      opacity: 1;
      position: absolute;
      transition: all 250ms ease-in;
      border-style: solid;
      border-color: red;
    }
    &.top-right{
      z-index: 2;
      top: 0;
      right: 0;
      width: 5px;
      height: 5px;
      border-width: 1px 1px 0 0;
      opacity: 1;
      position: absolute;
      transition: all 250ms ease-in;
      border-style: solid;
      border-color: red;
    }
    &.bottom-left{
      z-index: 2;
      bottom: 0;
      left:0;
      width: 5px;
      height: 5px;
      border-width: 0 0 1px 1px;
      opacity: 1;
      position: absolute;
      transition: all 250ms ease-in;
      border-style: solid;
      border-color: red;
    }
    &.bottom-right{
      z-index: 2;
      bottom: 0;
      right:0;
      width: 5px;
      height: 5px;
      border-width: 0 1px 1px 0;
      opacity: 1;
      position: absolute;
      transition: all 250ms ease-in;
      border-style: solid;
      border-color: red;
    }
  }
  .button{
    background: transparent ;
    border: none;
    cursor: pointer;
  }
}

</style>
