<template>
  <div class="home">
    <img alt="Vue logo" :src="img">
    <HelloWorld msg="Welcome to Your Vue.js App" />

  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
export default {
  name: 'Home',

  components: {
    HelloWorld
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
