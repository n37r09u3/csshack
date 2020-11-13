<template>
  <div id="app">

<div class="content-wrapper">
  <a href="#" class="corner-button"><span>Testing Hyperlink</span></a>
  <button class="corner-button"><span>Testing Button</span></button>
  <br />


  <a href="#" class="corner-button-vue"><span>Testing Hyperlink</span></a>
  <button class="corner-button-vue"><span>Testing Button</span></button>


</div>

  </div>
</template>

<script>

export default {
  name: 'About',
}
</script>

<style lang="scss">


$button_min_height: 30;
$button_min_width: 150;
$button_border_size: 15;
$button_font_size: 20;
$button_padding: 12px 20px;
$button_text_color: #A4CA6D;
$button_border_color: #A7A699;
$button_hover_text_color: #465159;
$button_hover_border_color: #A7A699;
$button_line_height: $button_min_height;

.corner-button-vue ,
.corner-button-vue  span {
  &:before,
  &:after {
    display: block;
    content: "1";
    width: #{$button_border_size}px;
    height: #{$button_border_size}px;
    position: absolute;
    background-color:red;
  }
}

.corner-button-vue {
    display: inline-block; //重要
    font-size: #{$button_font_size}px;
    margin: 20px;
     min-width: #{$button_min_width}px;
  min-height: #{$button_min_height}px;
   padding: #{$button_padding};
     border: none;
  position: relative;
cursor: pointer;
  line-height: #{$button_line_height}px;
  text-align: center;  //a
    box-sizing: content-box; //重要
    background: none; //button背景
    
       border: 2px solid transparent;//button 边框 2px？
        text-decoration:none; //a 下划线
          transition: 0.5s color;




  &:before {
    top: -2px;
    left: -2px;
    border-top: 2px solid $button_border_color;
    border-left: 2px solid $button_border_color;
    transition: 0.5s all;
  }
  &:after {
    top: -2px;
    right: -2px;
    border-top: 2px solid $button_border_color;
    border-right: 2px solid $button_border_color;
    transition: 0.5s all;
  }
  span {
    display: block;
    &:before {
      bottom: -2px;
      left: -2px;
      border-bottom: 2px solid $button_border_color;
      border-left: 2px solid $button_border_color;
      transition: 0.5s all;
    }
    &:after {
      bottom: -2px;
      right: -2px;
      border-bottom: 2px solid $button_border_color;
      border-right: 2px solid $button_border_color;
      transition: 0.5s all;
    }
  }
}


.corner-button,
.corner-button span {
  &:before,
  &:after {
    display: block;
    content: "";
    width: #{$button_border_size}px;
    height: #{$button_border_size}px;
    position: absolute;
  }
}



.corner-button {
  display: inline-block;
  font-size: #{$button_font_size}px;
  position: relative;
  min-width: #{$button_min_width}px;
  min-height: #{$button_min_height}px;
  margin: 20px;
  background: none;
  border: none;
  text-decoration:none;
  cursor: pointer;
  color: $button_text_color;
  padding: #{$button_padding};
  box-sizing: content-box;
  border: 2px solid transparent;
  text-align: center;
  line-height: #{$button_line_height}px;
  transition: 0.5s color;
  &:before {
    top: -2px;
    left: -2px;
    border-top: 2px solid $button_border_color;
    border-left: 2px solid $button_border_color;
    transition: 0.5s all;
  }
  &:after {
    top: -2px;
    right: -2px;
    border-top: 2px solid $button_border_color;
    border-right: 2px solid $button_border_color;
    transition: 0.5s all;
  }
  span {
    display: block;
    &:before {
      bottom: -2px;
      left: -2px;
      border-bottom: 2px solid $button_border_color;
      border-left: 2px solid $button_border_color;
      transition: 0.5s all;
    }
    &:after {
      bottom: -2px;
      right: -2px;
      border-bottom: 2px solid $button_border_color;
      border-right: 2px solid $button_border_color;
      transition: 0.5s all;
    }
  }
  &:hover {
    color: $button_hover_text_color;
    &:before,
    &:after {
      border-color: $button_hover_border_color;
      width: 100%;
      height: 100%;
    }
    span {
      &:before,
      &:after {
        border-color: $button_hover_border_color;
        width: 100%;
        height: 100%;
      }
    }
  }
}


</style>
