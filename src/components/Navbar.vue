<template>
  <nav id="mainNav" class="navbar navbar-default navbar-fixed-top"
       :class="{ 'navbar-default--transparent': navbarShouldTransparent }">
    <div class="container">
      <!-- Brand and toggle get grouped for better mobile display -->
      <div class="navbar-header">
        <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbar-collapse">
          <span class="sr-only"></span> 菜单 <i class="fa fa-bars"></i>
        </button>
        <a class="navbar-brand page-scroll" href="#page-top">Eva Cloud</a>
      </div>

      <!-- Collect the nav links, forms, and other content for toggling -->
      <div class="collapse navbar-collapse" id="navbar-collapse">
        <ul class="nav navbar-nav navbar-right">
          <li>
            <a class="page-scroll" href="#home">首页</a>
          </li>
          <li>
            <a class="page-scroll" href="#features">解决方案</a>
          </li>
          <li>
            <a class="page-scroll" href="#about">关于</a>
          </li>
          <li>
            <a class="page-scroll" href="#doc">开发文档</a>
          </li>
        </ul>
      </div>
      <!-- /.navbar-collapse -->
    </div>
    <!-- /.container-fluid -->
  </nav>
</template>

<script>
  export default {
    name: 'Navbar',

    data() {
      return {
        navbarShouldTransparent: true
      }
    },

    methods: {
      handleScroll () {
        this.navbarShouldTransparent = window.scrollY === 0
      }
    },

    mounted () {
      window.addEventListener('scroll', this.handleScroll)
    },

    beforeDestory () {
      window.removeEventListener('scroll', this.handleScroll)
    }
  }
</script>

<style lang="scss">
  .navbar-default {
    background-color: white;
    border-color: rgba(34, 34, 34, 0.05);
    -webkit-transition: all 0.35s;
    -moz-transition: all 0.35s;
    transition: all 0.35s;
    font-family: 'Catamaran', 'Helvetica', 'Arial', 'sans-serif';
    font-weight: 200;
    letter-spacing: 1px;
  }

  .navbar-default .navbar-header .navbar-brand {
    font-family: 'Catamaran', 'Helvetica', 'Arial', 'sans-serif';
    font-weight: 200;
    letter-spacing: 1px;
    color: #fdcc52;
  }

  .navbar-default .navbar-header .navbar-brand:hover,
  .navbar-default .navbar-header .navbar-brand:focus {
    color: #fcbd20;
  }

  .navbar-default .navbar-header .navbar-toggle {
    font-size: 12px;
    color: #222222;
    padding: 8px 10px;
  }

  .navbar-default .nav > li > a {
    font-family: 'Lato', 'Helvetica', 'Arial', 'sans-serif';
    text-transform: uppercase;
    letter-spacing: 2px;
    font-size: 11px;
  }

  .navbar-default .nav > li > a,
  .navbar-default .nav > li > a:focus {
    color: #222222;
  }

  .navbar-default .nav > li > a:hover,
  .navbar-default .nav > li > a:focus:hover {
    color: #fdcc52;
  }

  .navbar-default .nav > li.active > a,
  .navbar-default .nav > li.active > a:focus {
    color: #fdcc52 !important;
    background-color: transparent;
  }

  .navbar-default .nav > li.active > a:hover,
  .navbar-default .nav > li.active > a:focus:hover {
    background-color: transparent;
  }

  .navbar-default--transparent {
    @media (min-width: 768px) {
      background-color: transparent;
      border-color: transparent;

      .navbar-header .navbar-brand {
        color: rgba(255, 255, 255, 0.7);
      }
      .navbar-header .navbar-brand:hover,
      .navbar-header .navbar-brand:focus {
        color: white;
      }
      .nav > li > a,
      .nav > li > a:focus {
        color: rgba(255, 255, 255, 0.7);
      }
      .nav > li > a:hover,
      .nav > li > a:focus:hover {
        color: white;
      }
      &.affix {
        background-color: white;
        border-color: rgba(34, 34, 34, 0.1);
      }
      &.affix .navbar-header .navbar-brand {
        color: #222222;
      }
      &.affix .navbar-header .navbar-brand:hover,
      &.affix .navbar-header .navbar-brand:focus {
        color: #fdcc52;
      }
      &.affix .nav > li > a,
      &.affix .nav > li > a:focus {
        color: #222222;
      }
      &.affix .nav > li > a:hover,
      &.affix .nav > li > a:focus:hover {
        color: #fdcc52;
      }
    }
  }
</style>