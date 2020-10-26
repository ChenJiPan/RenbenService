<template>
  <div id="app">
    <HomePC v-if="isMobile == false" />
    <HomeM v-if="isMobile == true" />
  </div>
</template>

<script>
  import HomePC from './components/Home/HomePC.vue'
  import HomeM from './components/Home/HomeM.vue'

  export default {
    name: 'App',
    data() {
      return {
        isMobile: true
      }
    },
    components: {
      HomePC,
      HomeM
    },
    mounted() {
      this.isMobile = this.judgeIsMobile() ? true : false
    },
    methods: {
      judgeIsMobile() {
        let flag = navigator.userAgent.match(
          /(phone|pad|pod|iPhone|iPod|ios|iPad|Android|Mobile|BlackBerry|IEMobile|MQQBrowser|JUC|Fennec|wOSBrowser|BrowserNG|WebOS|Symbian|Windows Phone)/i
        )
        return flag;
      }
    }
  }
</script>

<style>

</style>
