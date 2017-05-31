<template>
  <footer>
    <div class="container">
      <p>&copy; 2017 Eva Tech. All Rights Reserved.</p>
      <ul class="list-inline">
        <li>
          <a href="#">政策</a>
        </li>
        <li>
          <a href="#">网站地图</a>
        </li>
        <li>
          <a href="#">常见问题</a>
        </li>
      </ul>
    </div>
  </footer>
</template>

<script>
  export default {
    name: 'Footerbar'
  }
</script>

<style lang="scss">
  footer {
    background-color: #222222;
    padding: 25px 0;
    color: rgba(255, 255, 255, 0.3);
    text-align: center;
  }
  footer p {
    font-size: 12px;
    margin: 0;
  }
  footer ul {
    margin-bottom: 0;
  }
  footer ul li a {
    font-size: 12px;
    color: rgba(255, 255, 255, 0.3);
  }
  footer ul li a:hover,
  footer ul li a:focus,
  footer ul li a:active,
  footer ul li a.active {
    text-decoration: none;
  }
</style>