<template>
  <div>
    <b-navbar fixed="top" toggleable="lg" type="dark" variant="dark">
      <b-navbar-brand href="/">
        KKZoo
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse" />

      <b-collapse id="nav-collapse" is-nav> 
        <!--右揃えのナビゲーションアイテム--> 
        <b-navbar-nav class="ml-auto"> 
          <b-nav-item v-scroll-to="'#top'">
            TOP
          </b-nav-item> 
          <b-nav-item v-scroll-to="'#myprof'">
            My Profile
          </b-nav-item> 
          <b-nav-item v-scroll-to="'#skill'">
            Skills
          </b-nav-item>
        </b-navbar-nav> 
      </b-collapse> 
    </b-navbar>
  </div>
</template>>