<template>
  <div class="home">

    <div class="arwes">
      <div class="border top"></div>
      <div class="border bottom"></div>
      <div class="border right"></div>
      <div class="border left"></div>
      <div class="corner">

      </div>
      <div class="corner">

      </div>
      <div class="corner">

      </div>
      <div class="corner">

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

  }
  .button{
    background: transparent ;
    border: none;
    cursor: pointer;
  }
}

</style>
