<template>
  <section class="contact bg-primary">
    <div class="container">
      <h2>在社交网络 <i class="fa fa-heart"></i> 关注我们！</h2>
      <ul class="list-inline list-social">
        <li class="social-twitter">
          <a href="#"><i class="fa fa-twitter"></i></a>
        </li>
        <li class="social-facebook">
          <a href="#"><i class="fa fa-facebook"></i></a>
        </li>
        <li class="social-google-plus">
          <a href="#"><i class="fa fa-google-plus"></i></a>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
  export default {
    name: 'SocialSection'
  }
</script>

<style lang="scss">
  section.contact {
    text-align: center;
  }
  section.contact h2 {
    margin-top: 0;
    margin-bottom: 25px;
  }
  section.contact h2 i {
    color: #dd4b39;
  }
  section.contact ul.list-social {
    margin-bottom: 0;
  }
  section.contact ul.list-social li a {
    display: block;
    height: 80px;
    width: 80px;
    line-height: 80px;
    font-size: 40px;
    border-radius: 100%;
    color: white;
  }
  section.contact ul.list-social li.social-twitter a {
    background-color: #1da1f2;
  }
  section.contact ul.list-social li.social-twitter a:hover {
    background-color: #0d95e8;
  }
  section.contact ul.list-social li.social-facebook a {
    background-color: #3b5998;
  }
  section.contact ul.list-social li.social-facebook a:hover {
    background-color: #344e86;
  }
  section.contact ul.list-social li.social-google-plus a {
    background-color: #dd4b39;
  }
  section.contact ul.list-social li.social-google-plus a:hover {
    background-color: #d73925;
  }
</style>