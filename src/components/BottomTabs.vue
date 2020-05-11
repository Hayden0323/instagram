<template>
  <div class="bottom-tabs">
    <span><i class="fa fa-home"></i></span>
    <span><i class="fa fa-search"></i></span>
    <span><i class="fa fa-instagram"></i></span>
    <span><i class="fa fa-heart-o"></i></span>
    <span><i class="fa fa-user-o"></i></span>
  </div>
</template>


<style lang='scss'>
.bottom-tabs {
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: 10;
  display: flex;
  border-top: 1px solid #eee;
  height: 64px;
  background-color: white;
  font-size: 20px;
}
.bottom-tabs span {
  display: flex;
  flex: 1;
  justify-content: center;
  align-items: center;
}
</style>