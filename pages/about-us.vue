<template>
  <div class="core-team">
    <div class="title-biz">
      <h3>core team</h3>
    </div>
    <div class="container">
      <div class="row">
        <div class="col-12">
          <div id="circle-shape-example">
            <img src="~static/images/sudip_saha.png" class="curve" />
            <p class="txTeam">
              Mr Sudip Saha -Result Oriented Executive with 24 years of IT
              Delivery Experience, and 10+ years of Leadership Experience
              inAccenture &amp; LogicaCMG. Love to dig customer problems and
              solve them with modern technology. I create, scale &amp;optimize
              solution to solve customer business problems.
            </p>
          </div>
        </div>
        <div class="col-12">
          <div id="circle-shape-example">
            <img src="~static/images/sudhir_mittal.jpg" class="curve" />
            <p class="txTeam">
              Mr. Sudhir Mittal an Alumni of IIT and IIM having extensive
              experience more than 32 years with highly engineered Information
              Systems which required deep understanding of critical business
              drivers in multi Industries and highly success in seizing control
              of critical problems areas and delivering on customer commitments
              . Lead and motivated world wide teams comprised from 20 to 200 and
              managed.
            </p>
          </div>
        </div>
        <div class="col-12">
          <div id="circle-shape-example">
            <img src="~static/images/shreya.png" class="curve" />
            <p class="txTeam">
              Dr. Sreya Experienced Professor with a demonstrated history of
              working in the computer software industry. Skilled in E-Learning,
              AI,Data Analysis, Lecturing, Instructional Design, and Science.
              Strong education professional with a Doctor of Philosophy (Ph.D.)
              focused in E-Healthcare in Rural India from University of
              Rajasthan.
            </p>
          </div>
        </div>
        <div class="col-12">
          <div id="circle-shape-example">
            <img
              src="https://cdn1.iconfinder.com/data/icons/technology-devices-2/100/Profile-512.png"
              class="curve"
            />
            <p class="txTeam">
              Arindam Roy, has over 13 years of experience, having worked with
              leading global advertising agencies - with a diverse knowledge in
              both mainline and digital, across Delhi and Gurgaon. Over the
              years, his role has involved copywriting for brands and content
              writing - essentially print ads, television commercials,
              brochures, outdoor hoardings, radio jingles and Point of sale
              collaterals.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {};
</script>

<style scoped>
.core-team {
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
}

@media screen and (max-width: 768px) {
  .core-team {
    background-size: cover;
    background-repeat: no-repeat;
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

.image-team {
  border-radius: 50%;
  width: 120px;
  display: block;
  margin-left: auto;
  margin-right: auto;
  margin-bottom: 20px;
}

.card-team {
  background: white;
  border-radius: 5px;
  margin: 8px;
  padding: 4px 4px;
  text-align: center;
  min-height: 330px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  box-shadow: 6px 6px 3px 0 rgba(51, 192, 145, 0.2);
}

@media (min-width: 37.5em) and (max-width: 768px) {
  .card-team {
    min-height: 455px;
  }
}

@media (min-width: 769px) and (max-width: 1024px) {
  .card-team {
    min-height: 376px;
  }

  .core-team {
    min-height: 84vh;
  }
}

.txTeam {
  text-align: justify;
  font-size: 14px;
}

#circle-shape-example {
  background: white;
  border-radius: 5px;
  padding: 4px 4px;
  box-shadow: 6px 6px 3px 0 rgba(51, 192, 145, 0.2);
  min-height: 130px;
  margin: 10px;
  width: 80%;
  margin-left: 10%;
}

@media screen and (max-width: 37.5em) {
  #circle-shape-example {
    margin-left: 0;
    width: 100%;
  }
}

#circle-shape-example .curve {
  height: auto;
  float: left;
  margin-right: 2rem;
  border-radius: 50%;
  -webkit-shape-outside: circle();
  shape-outside: circle();
}

.curve {
  width: 120px;
}
</style>