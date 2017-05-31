<template>
  <header>
    <div class="container">
      <div class="row">
        <div class="col-sm-7">
          <div class="header-content">
            <div class="header-content-inner">
              <h1>云接入从未如此简单</h1>
              <p>只需简单几步，即可让你的设备拥有自己的云大脑.</p>
              <a href="#" class="btn btn-outline btn-xl">立即申请试用</a>
            </div>
          </div>
        </div>
        <div class="col-sm-5">
          <div class="header-content">
            <div class="header-content-inner">
              <img src="~src/assets/img/demo-screen-1.jpg" class="img-responsive" alt="">
            </div>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
  export default {
    name: 'HeaderSection'
  }
</script>

<style lang="scss">
  @import '~src/scss/init';
  header {
    padding-top: 100px;
    position: relative;
    width: 100%;
    min-height: auto;
    overflow-y: hidden;
    background: url("~src/assets/img/bg-pattern.png"), #7b4397;
    /* fallback for old browsers */
    background: url("~src/assets/img/bg-pattern.png"), linear-gradient(to left, $purple, $red);
    /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
    color: white;
  }
  header .header-content {
    text-align: center;
    padding: 50px 0;
    position: relative;
  }
  header .header-content .header-content-inner {
    position: relative;
    max-width: 500px;
    margin: 0 auto;
  }
  header .header-content .header-content-inner h1 {
    margin-top: 0;
    margin-bottom: 30px;
    font-size: 30px;
  }
  header .header-content .header-content-inner .list-badges {
    margin-bottom: 25px;
  }
  header .header-content .header-content-inner .list-badges img {
    height: 50px;
    margin-bottom: 25px;
  }
  header .device-container {
    max-width: 300px;
    margin: 0 auto 100px;
  }
  header .device-container .screen img {
    border-radius: 3px;
  }
  @media (min-width: 768px) {
    header {
      padding-top: 0;
      min-height: 100%;
    }
    header .header-content {
      text-align: left;
      padding: 0;
      height: 100vh;
    }
    header .header-content .header-content-inner {
      max-width: none;
      margin: 0;
      position: absolute;
      top: 50%;
      transform: translateY(-50%);
    }
    header .header-content .header-content-inner h1 {
      font-size: 35px;
    }
    header .device-container {
      max-width: none;
      max-height: calc(0vh);
      margin: 100px auto 0;
    }
  }
  @media (min-width: 992px) {
    header .header-content .header-content-inner h1 {
      font-size: 50px;
    }
  }
</style>