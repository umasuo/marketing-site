<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-lg-12 text-center">
          <div class="section-heading">
            <h2>为什么选择 Eva Cloud</h2>
            <!--<p class="text-muted">没有副标题的话删了算了。。。</p>-->
            <hr>
          </div>
        </div>
      </div>

      <div class="row vcenter feature-block-img-text">
        <div class="col-md-6">
          <img class="feature-block-img-text__img" src="https://static2.tuyacn.com/static/portal/pc/cn/images/solution/big_electrical/why1@2x.040b1f16.png">
        </div>
        <div class="col-md-6">
          <h3 class="feature-block-img-text__title">
            产品适用于全球163个国家
            <br>
            助力中国家电企业出海
          </h3>
          <p class="feature-block-img-text__desc">
            当产品接入TUYA，你将拥有全球范围的涂鸦云服务，提供基于阿里云／亚马逊产品的全球高扩展的互联网架构方案。通过出海实现产品溢价，拓展海外的业务通道。
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    name: 'FeaturesWithImgSection'
  }
</script>

<style lang="scss">
  .feature-block-img-text {
    &__img {
      max-width: 100%;
      max-height: 100%;
    }

    &__title {
      font-size: 30px;
      font-weight: 200;
      letter-spacing: 1px;
    }
  }
</style>