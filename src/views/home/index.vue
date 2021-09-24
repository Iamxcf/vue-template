<template>
  <div class="home">
    <img alt="Vue logo" :src="img">
    <svg-icon icon-class="user" />

  </div>
</template>

<script>
export default {
  name: 'Home',

  components: {

  },
  data(){
    return {
      img: require('@/assets/logo.png')
    }
  },
  created(){
    console.log('process.env.NODE_ENV :>> ', process.env.VUE_APP_BASE_API)
  }
}
</script>
<style lang="scss" scoped>
.home{
  background: #000;
  height: 100vh;
  width: 100vh;
}
</style>
