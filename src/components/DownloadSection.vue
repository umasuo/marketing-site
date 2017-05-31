<template>
  <section class="download bg-primary text-center">
    <div class="container">
      <div class="row">
        <div class="col-md-8 col-md-offset-2">
          <h2 class="section-heading">扯一些广告语，然后引导点击按钮体验</h2>
          <p>每个新用户提供一个月免费体验时间，吧啦吧啦吧啦！按钮可以换成别的。</p>
          <div class="badges">
            <a class="badge-link" href="#"><img src="~src/assets/img/google-play-badge.svg" alt=""></a>
            <a class="badge-link" href="#"><img src="~src/assets/img/app-store-badge.svg" alt=""></a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    name: 'DownloadSection'
  }
</script>

<style lang="scss">
  @import '~src/scss/init';

  section.download {
    padding: 150px 0;
    position: relative;
  }
  section.download h2 {
    margin-top: 0;
    font-size: 50px;
  }
  section.download .badges .badge-link {
    display: block;
    margin-bottom: 25px;
  }
  section.download .badges .badge-link:last-child {
    margin-bottom: 0;
  }
  section.download .badges .badge-link img {
    height: 60px;
  }
  @media (min-width: 768px) {
    section.download .badges .badge-link {
      display: inline-block;
      margin-bottom: 0;
    }
  }
  @media (min-width: 768px) {
    section.download h2 {
      font-size: 70px;
    }
  }
</style>