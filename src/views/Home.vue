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

      <div class="frame">
        <button class="button">按钮</button>

      </div>


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
.frame{
  background: transparent ;
  transition: background-color 250ms ease-in;
}
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
      top: -1px;
      left: -1px;
      width: 5px;
      height: 5px;
      border-width: 1px 0 0 1px;
      opacity: 1;
      position: absolute;
      transition: all 250ms ease-in;
      border-style: solid;
      border-color: #acf9fb;
      box-shadow: 0 0 4px -2px rgba(172,249,251,0);
    }
    &.top-right{
      z-index: 2;
      top: -1px;
      right: -1px;
      width: 5px;
      height: 5px;
      border-width: 1px 1px 0 0;
      opacity: 1;
      position: absolute;
      transition: all 250ms ease-in;
      border-style: solid;
      border-color: #acf9fb;
      box-shadow: 0 0 4px -2px rgba(172,249,251,0);
    }
    &.bottom-left{
      z-index: 2;
      bottom: -1px;
      left:-1px;
      width: 5px;
      height: 5px;
      border-width: 0 0 1px 1px;
      opacity: 1;
      position: absolute;
      transition: all 250ms ease-in;
      border-style: solid;
      border-color: #acf9fb;
      box-shadow: 0 0 4px -2px rgba(172,249,251,0);
    }
    &.bottom-right{
      z-index: 2;
      bottom: -1px;
      right:-1px;
      width: 5px;
      height: 5px;
      border-width: 0 1px 1px 0;
      opacity: 1;
      position: absolute;
      transition: all 250ms ease-in;
      border-style: solid;
      border-color: #acf9fb;
      box-shadow: 0 0 4px -2px rgba(172,249,251,0);
    }
  }
  .button{
    color: #acf9fb;
    display: block;
    line-height: 1;
    background: transparent ;
    border: none;
    cursor: pointer;
    vertical-align: middle;
    margin: 0;
    padding: 10px 20px;
    outline: none;
  }
}

</style>
