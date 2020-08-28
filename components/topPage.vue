<template>
  <section class="top-page">
    <img src="~/assets/topPageImage.jpeg" class="top-page-image">
    <p class="top-page-title">
      KKZoo's SAMPLE PAGE
    </p>
    <p class="top-page-text">
      down scroll page
    </p>        
  </section>
</template>

<style>
.top-page{
    position: relative;
    display: flex;
    justify-content: center;
}

.top-page-image{
    width: 100%;    
}

.top-page-title{
    position: absolute;
    color: rgb(156, 162, 49);
    font-size: 30px;
    top: 30%;
}

.top-page-text{
    position: absolute;
    color: white;
    bottom: 0%;
}
</style>