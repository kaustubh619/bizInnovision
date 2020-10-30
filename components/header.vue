<template>
  <div style="position: fixed; top: 0; left: 0; width: 100%; z-index: 10">
    <nav>
      <div>
        <nuxt-link to="/"
          ><img src="~static/images/biz1.jpg" class="nav-logo"
        /></nuxt-link>
      </div>
      <ul class="nav-links">
        <li><nuxt-link to="/">home</nuxt-link></li>
        <li><nuxt-link to="/about-us">about us</nuxt-link></li>
        <li><nuxt-link to="/our-clients">our clients</nuxt-link></li>
        <li><nuxt-link to="">contact</nuxt-link></li>
      </ul>
      <div class="burger">
        <div class="line1"></div>
        <div class="line2"></div>
        <div class="line3"></div>
      </div>
    </nav>
  </div>
</template>

<script>
  export default {
    mounted() {
      const navSlide = () => {
        const burger = document.querySelector(".burger");
        const nav = document.querySelector(".nav-links");
        const navLinks = document.querySelector(".nav-links li");

        burger.addEventListener("click", () => {
          nav.classList.toggle("nav-active");
          burger.classList.toggle("toggle");
        });

        $(".nav-links li").click(function () {
          nav.classList.toggle("nav-active");
        });
      };
      navSlide();
    },
  };
</script>

<style>
nav {
  display: flex;
  justify-content: space-around;
  align-items: center;
  min-height: 8vh;
  background: white;
}

.nav-logo {
  width: 170px;
}

.nav-links {
  list-style: none;
  display: flex;
  justify-content: space-around;
  width: 30%;
}

.nav-links a {
  color: black;
}

.nav-links a:hover {
  color: grey;
}

.burger {
  display: none;
}

.burger div {
  width: 25px;
  height: 3px;
  background-color: black;
  margin: 5px;
  cursor: pointer;
  transition: all 0.5s ease-in;
}

@media screen and (max-width: 1024px) {
  .nav-links {
    width: 50%;
  }
}

@media screen and (max-width: 768px) {
  .burger {
    position: absolute;
    top: 2vh;
    right: 2vh;
  }

  body {
    overflow-x: hidden;
  }

  nav {
    justify-content: space-around;
  }

  .nav-links {
    position: absolute;
    right: 0px;
    height: 100vh;
    top: 0vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 50%;
    transform: translateX(100%);
    transition: transform 0.5s ease;
    background: #5d4954;
    opacity: 0.95;
  }

  .nav-links a {
    color: white;
  }

  .nav-links li {
    opacity: 1;
  }

  .burger {
    display: block;
  }

  .toggle .line1 {
    transform: rotate(-45deg) translate(-5px, 6px);
  }
  .toggle .line2 {
    opacity: 0;
  }
  .toggle .line3 {
    transform: rotate(45deg) translate(-5px, -6px);
  }
}
</style>