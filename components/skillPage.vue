<template>
  <section id="skill">
    <span class="skill-desgin">
    <img src="~/assets/skill-icon.png" class="skill-icon">
    <h2 class="skill-page-title">
      Skills
    </h2>
    </span>
    <div class="container">
      <div class="row">
        <div class="col-sm-4">
          <div class="row">
            <div class="col-12 margin-logo">
              <span class="underline">
                Vue.js
              </span>
            </div>
            <div class="col-12">
              <img src="~/assets/vue_logo.png" class="vue-logo">
            </div>
          </div>
        </div>
        <div class="col-sm-4">
          <div class="col-12 margin-logo">
            <span class="underline">
              CSS
            </span>
          </div>
          <div class="col-12">
            <img src="~/assets/css_logo.svg" class="css-logo">
          </div>
        </div>
        <div class="col-sm-4">
          <div class="col-12 margin-logo">
            <span class="underline">
              Bootstrap Vue
            </span>
          </div>
          <div class="col-12">
            <img src="~/assets/bootstrap_vue_logo.png" class="bootstrap-logo">
          </div>
        </div>
      </div>
    </div>
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

.margin-logo{
    margin: 10px;
}

.vue-logo{
    width: 100%;
}

.css-logo{
    width: 100%;
}

.bootstrap-logo{
    width: 100%;
}
</style>>