<template>
  <div class="header">
    <div class="left">
      <div class="header_button" @click='click_home'>
        <i class="fas fa-home"></i>
      </div>
    </div>
    <div class="center_title" @click='click_home'>
      <span>Trello?</span>
    </div>
    <div class="right">
      <div class="header_button"  @click='click_add'>
        <i class="fas fa-plus-circle"></i>
      </div>
      <div class="header_button" @click='click_information'>
        <i class="fas fa-info-circle"></i>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods:{
    click_home () {
      router.push('/')
    },
    click_add () {
      alert('click_add!!')
    },
    click_information () {
      alert('click_information')
    }
  }
}
</script>
<style lang="css">
.header{
  display: inline-block;
  position: fixed;  /* 画面上部に固定 */
  width: 100%;
  height: 50px;
  top: 0;
  right: 0;
  left: 0;
  background-color: rgb(66, 201, 173);
}
.header_button{
  display: inline-block;
  font-size: 40px;
  text-align: center;
  width: 49px;
  height: 49px;
  border-radius: 5px;
  background-color: rgb(100, 217, 192);
}
.left{
  float: left;
}
.center_title{
  font-size: 40px;
  font-weight: bold;
  display:inline-block;
  text-align: center;
  transition: 1.0s ;
}
.center_title:hover{
  color: rgb(227, 227, 227);
}
.right{
  float: right;
}
</style>
