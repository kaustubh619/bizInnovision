<template>
  <div>
    <Header />
    <Nuxt />
    <Footer />
  </div>
</template>

<script>
  import Header from "@/components/header.vue";
  import Footer from "@/components/footer.vue";
  export default {
    components: {
      Header,
      Footer,
    },
  };
</script>

<style>
html,
body {
  font-family: "Bills Mafia Regular" !important;
  font-weight: normal;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0px;
}

a {
  text-decoration: none !important;
}

.nav-active {
  transform: translateX(0%);
}
</style>
