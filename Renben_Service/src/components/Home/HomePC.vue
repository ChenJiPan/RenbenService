<template>
  <div>
    <!-- 背景 -->
    <div class="backBoxBG"></div>
    <div id="HomeContentBox_PC">
      <!-- 标题栏 -->
      <img class="LogoImgBox" src="../../../static/img/logo.png">
      <div class="downloadHint">
        <span>App 下载</span>
        <p></p>
      </div>

      <div class="contentBox_PC">
        <img class="downloadAPP_PC" src="../../../static/img/loadIOS.png" @click="pushLoadIOSApp">
        <img class="downloadAPP_PC" src="../../../static/img/loadAndroid.png" @click="pushLoadAndroidApp">
      </div>

      <!-- 底部内容 -->
      <div class="hintBox">
        <span style="text-align: left;">服务协议&emsp;&emsp;隐私政策</span>
        <span style="float: right;text-align: right;">粤ICP备19038094号&emsp;深圳普绪克网络科技有限公司</span>
      </div>

    </div>

  </div>

  </div>

</template>

<script>
  export default {
    methods: {
      //下载iOSAPP
      pushLoadIOSApp() {
        window.location.href = 'https://apps.apple.com/cn/app/%E8%81%8A%E6%9C%BA-%E5%90%8C%E5%9F%8E%E7%9B%B8%E4%BA%B2%E4%BA%A4%E5%8F%8B%E8%81%8A%E5%A4%A9%E7%BA%A6%E4%BC%9A%E8%BD%AF%E4%BB%B6%E8%81%8A%E6%9C%BA/id1467874323'
      },
      //下载安卓APP
      pushLoadAndroidApp() {

      }
    }
  }
</script>

<style>
</style>
