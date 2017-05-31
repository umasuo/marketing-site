<template>
  <section id="features" class="features">
    <div class="container">
      <div class="row">
        <div class="col-lg-12 text-center">
          <div class="section-heading">
            <h2>Eva Cloud 的优势</h2>
            <p class="text-muted">没有副标题的话删了算了。。。</p>
            <hr>
          </div>
        </div>
      </div>
      <div class="row">
        <!--<div class="col-md-4">-->
          <!--<div class="device-container">-->
            <!--<div class="device-mockup iphone6_plus portrait white">-->
              <!--<div class="device">-->
                <!--<div class="screen">-->
                  <!--&lt;!&ndash; Demo image for screen mockup, you can put an image here, some HTML, an animation, video, or anything else! &ndash;&gt;-->
                  <!--<img src="~src/assets/img/demo-screen-1.jpg" class="img-responsive" alt=""> </div>-->
                <!--<div class="button">-->
                  <!--&lt;!&ndash; You can hook the "home button" to some JavaScript events or just remove it &ndash;&gt;-->
                <!--</div>-->
              <!--</div>-->
            <!--</div>-->
          <!--</div>-->
        <!--</div>-->
        <div class="col-md-12">
          <div class="container-fluid">
            <div class="row">
              <div class="col-md-4">
                <div class="feature-item">
                  <i class="icon-screen-smartphone text-primary"></i>
                  <h3>极简接入</h3>
                  <p class="text-muted">Eva Cloud 云平台，作为SAAS平台提供服务。采取一键式申请，申请即可使用的方式，简化申请审核流程，简化设备接入方式，提升硬件开发团队的效率</p>
                </div>
              </div>
              <div class="col-md-4">
                <div class="feature-item">
                  <i class="icon-camera text-primary"></i>
                  <h3>安全，稳定，高效</h3>
                  <p class="text-muted">云平台采用业界领先的技术进行开发。部署，目前采用的基础架构为：kubernetes，docker，微服务，同时云平台运行在AWS上，能够提供更稳定，安全的云服务。
                  <p class="text-muted">实时的预警和状态监控也极大的提升了云服务的可靠性</p>
                </div>
              </div>
              <div class="col-md-4">
                <div class="feature-item">
                  <i class="icon-present text-primary"></i>
                  <h3>灵活的自定义功能</h3>
                  <p class="text-muted">每个团队的核心竞争力必然会有自己独特的功能，Eva云平台提供了每个团队定义自己业务功能的方案，让你不必再部署独立的一套云服务</p>
                </div>
              </div>
            </div>
            <div class="row">
              <div class="col-md-4">
                <div class="feature-item">
                  <i class="icon-lock-open text-primary"></i>
                  <h3>实时的数据分析</h3>
                  <p class="text-muted">实时的数据分析，数据报表能够更有效的为团队提供各方面的决策支持</p>
                </div>
              </div>
              <div class="col-md-4">
                <div class="feature-item">
                  <i class="icon-lock-open text-primary"></i>
                  <h3>设备协作，单品价值提升</h3>
                  <p class="text-muted">单兵作战的时代终究会远去，集体协作的方式能够极大的放大单品的价值，能够更好的为用户服务。</p>
                  <p class="text-muted">Eva云平台为设备间的协作，团队间的协作提供了可能</p>
                </div>
              </div>
              <div class="col-md-4">
                <div class="feature-item">
                  <i class="icon-lock-open text-primary"></i>
                  <h3>带按钮的 Feature</h3>
                  <p class="text-muted">单兵作战的时代终究会远去，集体协作的方式能够极大的放大单品的价值，能够更好的为用户服务。</p>
                  <a class="btn btn-outline btn-primary btn-xl">立即申请试用</a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    name: 'FeaturesSection'
  }
</script>

<style lang="scss">
  section.features .section-heading {
    margin-bottom: 100px;
  }
  section.features .section-heading h2 {
    margin-top: 0;
  }
  section.features .section-heading p {
    margin-bottom: 0;
  }
  section.features .device-container,
  section.features .feature-item {
    max-width: 300px;
    margin: 0 auto;
  }
  section.features .device-container {
    margin-bottom: 100px;
  }
  @media (min-width: 992px) {
    section.features .device-container {
      margin-bottom: 0;
    }
  }
  section.features .feature-item {
    text-align: center;
    margin-bottom: 100px;
  }
  section.features .feature-item h3 {
    font-size: 30px;
  }
  section.features .feature-item i {
    font-size: 80px;
    background: -webkit-linear-gradient(to left, #7b4397, #dc2430);
    background: linear-gradient(to left, #7b4397, #dc2430);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
  @media (min-width: 992px) {
    section.features .device-container,
    section.features .feature-item {
      max-width: none;
    }
  }
</style>