<template>
  <section id="top" class="top-page">
    <transition name="slide">
      <span :key="products[product]">
        <img :src="products[product]" class="top-page-image">
      </span>
    </transition>
   
    <p class="top-page-title">
      KKZoo's SAMPLE PAGE
    </p>
    <span class="top-page-text">
      <p>
        scroll down page
      </p>
    </span>

    <img src="~/assets/left-icon.png" class="slide-before-button" @click="beforeSlide">
    <img src="~/assets/right-icon.png" class="slide-next-button" @click="nextSlide">
  </section>
</template>

<script>
export default {
  data: function() {
    return {
      product: 0,
      products: [
        require('@/assets/topPageImage-1.jpg'),
        require('@/assets/topPageImage-2.jpg'),
        require('@/assets/topPageImage-3.jpg'),
      ]
    }
  },
  methods: {
    nextSlide: function() {
      if(this.product < this.products.length - 1){
        this.product += 1
      }else{
        this.product = 0
      }
    },
    beforeSlide: function() {
      if(this.product > 0){
        this.product -= 1
      }else{
        this.product = this.products.length - 1
      }
    }
  }
}
</script>

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
    bottom: 0;
    text-align: center;
}

.slide-before-button {
  position: absolute;
  left: 0;
  top: 50%;
  width: 2rem;
}

.slide-next-button {
  position: absolute;
  right: 0;
  top: 50%;
  width: 2rem;
}

.slide-enter-active {
  transition: transform 0.75s
}
.slide-leave-active{
  transition: transform 0s
}
.slide-enter {
  transform: translateX(500px)
}
.slide-leave {
  transform: opacity 0
}
</style>