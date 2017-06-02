<template>
  <section class="guide-section">
    <div class="container">
      <div class="row">
        <div class="col-lg-12 text-center">
          <div class="section-heading">
            <h2>4步快速完成智能化</h2>
            <hr>
          </div>
        </div>
      </div>

      <div class="row text-center guide-section__steps">
        <div class="guide-section__step" @click="step = 1">
          1 成为开发者
        </div>
        <div class="guide-section__step"  @click="step = 2">
          2 成为开发者
        </div>
        <div class="guide-section__step"  @click="step = 3">
          3 成为开发者
        </div>
        <div class="guide-section__step"  @click="step = 4">
          4 成为开发者
        </div>
      </div>

      <div class="row">
        <div class="col-xs-12">
          <div class="panel panel-default guide-section__content">
            <div class="container-fluid">
              <div class="row vcenter">
                <div class="col-sm-8">
                  <h2 class="guide-section__title">{{ step }} 如何成为开发者</h2>
                  <p class="guide-section__desc">只需简单注册和信息填写，即可成为涂鸦智能云平台开发者。<br>涂鸦提供丰富开发工具，帮你快速实现智能化</p>

                  <div class="guide-section__feature-wrapper">
                      <div class="guide-section__feature">
                        <i class="fa fa-4x fa-bandcamp" aria-hidden="true"></i>
                        <p>文档中心</p>
                      </div>
                      <div class="guide-section__feature">
                        <i class="fa fa-4x fa-bandcamp" aria-hidden="true"></i>
                        <p>文档中心</p>
                      </div>
                  </div>
                </div>

                <div class="col-sm-4">
                  <a href="#" class="btn btn-xl btn-primary">立即注册，成为开发者</a>
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
    name: 'GuideSection',
    data () {
      return {
        step: 1
      }
    }
  }
</script>

<style lang="scss">
  @import '~src/scss/init';

  .guide-section {
    &__steps {
      display: flex;
      justify-content: space-around;
      margin: 50px 0;

      @media (min-width: 768px) {
        background-image: linear-gradient(to right, $primary-color 50%, transparent 50%);
        background-size: 30px 7px;
        background-repeat: repeat-x;
        background-position: center;
      }
    }

    &__step {
      color: $primary-color;
      border-radius: 50%;
      cursor: pointer;

      @media (min-width: 768px) {
        background-color: $primary-color;
        color: white;
        width: 100px;
        height: 100px;
        line-height: 100px;
      }
    }

    &__feature-wrapper {
      text-align: center;
      @media (min-width: 768px) {
        text-align: left;
      }
    }

    &__desc {
      text-align: left;
    }

    &__feature {
      display: inline-block;
      color: $primary-color;
      text-align: center;
      padding-right: 20px;
    }

    &__content {
      text-align: center;
      padding: 20px;
      
      @media (min-width: 768px) {
        text-align: left;
      }
    }
  }
</style>