<template>
  <section id="myprof" class="myprof-all">
    <span class="prof-desgin">
      <img src="~/assets/prof-icon.png" class="prof-icon">
      <h2 class="myprof-page-title">
        My Profile
      </h2>
    </span>
    <div class="row">
      <b-container class="col-12 d-flex justify-content-center">
        <img src="~/assets/mon.jpg" class="mon-image">
      </b-container>
      <b-container class="col-12 d-flex justify-content-center">
        <ul>
          <li>
            Author: KKZoo
          </li>
          <li>
            BirthDay: 5/2
          </li>
          <li>
            Country: Japan
          </li>
        </ul>
      </b-container>
    </div>
  </section>
</template>

<style>
.myprof-all{
  background: #6ff7ff;
  border-radius: 10%;
}

.myprof-page-title{
    left: 0%;
    margin-top: 5px;
    margin-left: 5px;
}

.prof-desgin{
  display: flex;
  margin-top: 30px;
  margin-bottom: 30px;
  margin-left: 20px;
}

.prof-icon{
  width: 3rem;
  height: 3rem;
}

.mon-image{
  width: 6em;
  height: 6em;
  border-radius: 50%;
  margin: 5px; 
}

ul{
  list-style: none;
}

li{
  margin: 5px;
}
</style>>