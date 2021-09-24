<template>
  <div class="home">
    {{ content }}

  </div>
</template>

<script>
export default {
  name: 'Home',

  components: {

  },
  data(){
    return {
      // img: require('@/assets/logo.png')
      content: '首页'
    }
  },
  created(){
    console.log('process.env.NODE_ENV :>> ', process.env.VUE_APP_BASE_API)
  }
}
</script>
<style lang="scss" scoped>
.home{
  height: 100vh;
  width: 100vh;
  background: $activeText;
}
</style>
