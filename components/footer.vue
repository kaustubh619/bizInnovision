<template>
  <div>
    <footer class="container">
      <div class="footer-biz">
        <nuxt-link to=""><img src="~static/images/fb.png" /></nuxt-link>
        <nuxt-link to=""><img src="~static/images/twitter.png" /></nuxt-link>
        <nuxt-link to=""><img src="~static/images/insta.png" /></nuxt-link>
        <nuxt-link to=""><img src="~static/images/linked.webp" /></nuxt-link>
        <nuxt-link to=""><img src="~static/images/pin.jpg" /></nuxt-link>
      </div>
      <p style="text-align: center">Copyright ©2020 All rights reserved</p>
    </footer>
  </div>
</template>

<script>
  export default {};
</script>

<style>
.footer-biz {
  display: flex;
  justify-content: center;
  align-items: center;
}

.footer-biz img {
  width: 40px;
  margin: 10px;
  border-radius: 50%;
}

@media screen and (max-width: 768px) {
  .footer-biz img {
    width: 24px;
  }
}
</style>