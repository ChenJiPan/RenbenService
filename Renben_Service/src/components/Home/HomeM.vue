<template>
  <div>
    <!-- 背景 -->
    <div class="backBoxBG"></div>
    <div id="HomeContentBox_M">
      <!-- 标题栏 -->
      <img class="LogoImgBox" src="../../../static/img/logo.png">
      <div class="downloadHint">
        <span>App 下载</span>
        <p></p>
      </div>

      <div class="contentBox_M">
        <img class="downloadAPP_M" src="../../../static/img/loadIOS.png" @click="pushLoadIOSApp">
        <img class="downloadAPP_M" style="margin-top: 10px;" src="../../../static/img/loadAndroid.png" @click="pushLoadAndroidApp">
      </div>

      <!-- 底部内容 -->
      <div class="hintBox">
        <p style="text-align: left;" @click="pushProtocol">服务协议&emsp;&emsp;隐私政策</p>
        <p style="text-align: center;margin-top: 20px;" @click="pushCompany">粤ICP备19038094号&emsp;深圳普绪克网络科技有限公司</p>
      </div>

    </div>
  </div>
</template>

<script>
  export default {
    methods: {
      //下载iOSAPP
      pushLoadIOSApp() {
        window.location.href =
          'https://apps.apple.com/cn/app/%E8%81%8A%E6%9C%BA-%E5%90%8C%E5%9F%8E%E7%9B%B8%E4%BA%B2%E4%BA%A4%E5%8F%8B%E8%81%8A%E5%A4%A9%E7%BA%A6%E4%BC%9A%E8%BD%AF%E4%BB%B6%E8%81%8A%E6%9C%BA/id1467874323'
      },
      //下载安卓APP
      pushLoadAndroidApp() {
        window.location.href = 'https://dev.psychelove.com/#/Privacy'
      },
      //跳转协议
      pushProtocol() {
        window.location.href = 'https://dev.psychelove.com/#/Privacy'
      },
      //跳转公司
      pushCompany() {
        window.location.href = 'https://beian.miit.gov.cn'
      }
    }
  }
</script>

<style>
</style>
