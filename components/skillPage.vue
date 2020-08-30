<template>
  <section id="skill">
    <span class="skill-desgin">
      <img src="~/assets/skill-icon.png" class="skill-icon">
      <h2 class="skill-page-title">
        Skills
      </h2>
    </span>
    <b-row>
    <b-container>
      <b-row>
        <b-col cols="6" sm="4">
          <b-container class="d-flex justify-content-center">
            <b-row>
              <b-col cols="12">
                <span class="underline">
                  Vue.js
                </span>
              </b-col>
              <b-col cols="12">
                <img src="~/assets/vue_logo.png" class="vue-logo">
              </b-col>
            </b-row>
          </b-container>
        </b-col>
        <b-col cols="6" sm="4">
          <b-container class="d-flex justify-content-center">
            <b-row>
              <b-col cols="12">
                <span class="underline">
                  CSS
                </span>
              </b-col>
              <b-col cols="12">
                <img src="~/assets/css_logo.svg" class="css-logo">
              </b-col>
            </b-row>
          </b-container>
        </b-col>
        <b-col cols="6" sm="4">
          <b-container class="d-flex justify-content-center">
            <b-row>
              <b-col cols="12">
                <span class="underline">
                  Bootstrap Vue
                </span>
              </b-col>
              <b-col cols="12">
                <img src="~/assets/bootstrap_vue_logo.png" class="bootstrap-logo">
              </b-col>
            </b-row>
          </b-container>
        </b-col>
      </b-row>
    </b-container>
      </b-row>
  </section>
</template>

<style>
.skill-page-title{
    left: 0%;
    margin-top: 5px;
    margin-left: 5px;
}

.skill-desgin{
  display: flex;
  margin-top: 30px;
  margin-bottom: 30px;
  margin-left: 20px;
}

.skill-icon{
  width: 3rem;
  height: 3rem;
}

.underline{
    border-bottom: 2px solid gray;
}

.vue-logo{
    width: 10rem;
    margin-top: 5px; 
}

.css-logo{
    width: 10rem;
    margin-top: 5px;
}

.bootstrap-logo{
    width: 10rem;
    margin-top: 5px;
}
</style>>