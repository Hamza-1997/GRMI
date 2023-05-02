<script>
// import WelcomeItem from './WelcomeItem.vue'
// import DocumentationIcon from './icons/IconDocumentation.vue'
// import ToolingIcon from './icons/IconTooling.vue'
// import EcosystemIcon from './icons/IconEcosystem.vue'
// import CommunityIcon from './icons/IconCommunity.vue'
import CustomButton from './Buttons/Button.vue'



export default {
  components: {
    CustomButton,
  },
  // methods: {
  //   handleButtonClick() {
  //     alert('Button clicked!');
  //   },
  // },
};
</script>

<template>
  <div class="hero-image">
    <!-- <img class="lg:w-2/6 md:w-3/6 w-5/6 mb-10 object-cover object-center" alt="hero" src={HeroImage} /> -->
    <!-- <img src='../assets/icons/HeroImage.png' /> -->

    <!-- <HeroImage /> -->
    <div class="container">

      <div class="row">
        <div class="hero-container w-100">
          <div class="hero-text w-100">
            <div class="C61 white" style="margin-bottom: 16px;">GeoHazards; Predict,Prepare, Protect.</div>

            <p class="M20 white" style="margin-bottom: 16px;">Promoting a sustainable environment
              through
              the
              development,
              generating applications, and <br />
              dissemination of Geohazard maps using advanced Geospatial Technology</p>
            <div>
            </div>
            <!-- <div class="col-lg-3 col-md-6 "> -->
            <!-- <div> -->

            <!-- <Button class="M16 me-lg-4 me-md-4 me-sm-4 me-xs-0" button-type="primary" button-text="View Water Level"
              style="width: 216px; height: 67px; background-color: #134A39;color: white;">Test</Button> -->

            <!-- label:"Big Button Label",
      type:"warning",
      size:"lg",
      active:"true",
      block:"true" -->
            <!-- </div> -->
          </div>
          <div>
            <CustomButton class="M16 white btn-success" btn-text="View Water Level" type="success" size="lg" />
            <!-- style="border-radius: 0;background-color: #134A39;border: none;width: 216px;height: 67px;"  -->


            <CustomButton class="M16 btn-outline" btn-text="View Dashboard" type="outline-secondary" size="lg"
              style="border-radius: 0;background-color: transparent;width: 216px;height: 67px;color: #EAF7F3;" />
          </div>

          <!-- <CustomButton class="M16 mt-2" button-type="primary" button-text="View Dashboard"
            style="width: 216px; height: 67px; background-color: transparent;color: white;border: 1px solid white;" /> -->


        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.hero-image {
  background-image: linear-gradient(rgba(0, 0, 0, 0), rgba(0, 0, 0, 0)), url('../assets/icons/HeroImage.png');
  /* background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)); */
  height: 100vh;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  /* position: relative; */
  /* margin-top: 105px; */
}

.hero-container {
  /* padding: 0 40px 0 40px; */
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  text-align: center;
}

.hero-text {
  /* height: 100vh; */
  padding: 0 40px 0 40px;
  /* position: absolute; */
  /* top: 50%; */
  /* left: 50%; */
  /* transform: translate(-50%, -50%); */
  color: white;
}

.hero-text button {
  border: none;
  outline: 0;
  display: inline-block;
  padding: 10px 25px;
  color: black;
  background-color: #ddd;
  text-align: center;
  cursor: pointer;
}

.hero-text button:hover {
  background-color: #555;
  color: white;
}

.btn-success {
  margin-right: 16px;
}

@media (max-width: 485px) {
  .btn-success {
    margin-right: 0;
  }

  /* margin-bottom: 16px; */
}

@media (max-width: 455px) {
  .btn-success {
    margin-bottom: 16px;
  }

  /* margin-bottom: 16px; */
}
</style>