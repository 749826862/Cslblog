<template>
  <div id="container">
    我的第一个nuxt应用
  </div>
</template>

<script>
export default {
  mounted(){
    let box = document.getElementById('container')
    let x = this.$velocity(box, {
      top: 500
    })
    console.log(x, 888)
    this.$velocity(box, {left: 300})
  }
}
</script>

<style>
#container {
  width: 300px;
  position: relative;
}

</style>
