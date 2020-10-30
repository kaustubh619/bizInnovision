<template>
  <div class="clients">
    <div class="title-biz">
      <h3>our clients</h3>
    </div>
    <div class="container-fluid">
      <div class="row">
        <div class="col-12">
          <div class="center">
            <div class="items">
              <img src="~static/images/clients/symbiosis_infra.png" />
            </div>
            <div class="items">
              <img src="~static/images/clients/advance_health_care.png" />
            </div>
            <div class="items">
              <img src="~static/images/clients/enviflow.jpg" />
            </div>
            <div class="items">
              <img src="~static/images/clients/isccm.png" />
            </div>
            <div class="items">
              <img src="~static/images/clients/vm_design.jpg" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    mounted() {
      $(".center").slick({
        centerMode: true,
        centerPadding: "0px",
        slidesToShow: 3,
        autoplay: true,
        autoplaySpeed: 2000,
        responsive: [
          {
            breakpoint: 768,
            settings: {
              arrows: true,
              centerMode: true,
              centerPadding: "0px",
              slidesToShow: 3,
            },
          },
          {
            breakpoint: 480,
            settings: {
              arrows: true,
              centerMode: true,
              centerPadding: "0px",
              slidesToShow: 1,
            },
          },
        ],
      });
    },
  };
</script>

<style scoped>
.clients {
  margin-top: 102px;
  background-image: url("~static/images/pexels-karolina-grabowska-4040654.jpg");
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
  min-height: 81vh;
  padding-bottom: 14px;

  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

@media screen and (max-width: 768px) {
  .clients {
    background-size: cover;
    background-repeat: no-repeat;
  }
}

@media screen and (max-width: 37.5em) {
  .clients {
    min-height: 74vh;
  }
}

.title-biz h3 {
  text-align: center;
  color: #1a3df0;
  font-size: 50px;
  margin: 0px;
  padding-top: 16px;
}

@media screen and (max-width: 1024px) {
  .title-biz h3 {
    font-size: 32px;
  }
}

@media screen and (max-width: 768px) {
  .title-biz h3 {
    font-size: 24px;
  }
}

@media screen and (max-width: 37.5em) {
  .title-biz h3 {
    font-size: 14px;
  }
}

.items img {
  width: 100%;
  padding: 20px;
}

.center {
  margin-left: 10%;
  width: 80%;
  margin-top: 40px;
}
</style>