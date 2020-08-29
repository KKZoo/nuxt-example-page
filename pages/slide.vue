<template>
  <div class="top-page">
    <transition name="slide">
      <span :key="products[product]">
        <img :src="products[product]" class="img-size">
      </span>
    </transition>

    <p class="top-page-title">
      KKZoo's SAMPLE PAGE
    </p>

    <button @click="beforeSlide" class="slide-before-button">
      前
    </button>
    <button @click="nextSlide" class="slide-next-button">
      次
    </button>
  </div>
</template>

<script>
export default {
  data: function() {
    return {
      product: 0,
      products: [
        require('@/assets/topPageImage.jpeg'),
        require('@/assets/mon.jpg'),
        require('@/assets/vue_logo.png'),
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
.slide-enter-active {
  transition: transform 0.75s
}
.slide-leave-active{
  transition: transform 0s
}
.slide-enter {
  transform: translateX(300px)
}
.slide-leave {
  transform: opacity 0
}

.top-page{
  position: relative;
  display: flex;
  justify-content: center;
}

.slide-before-button {
  position: absolute;
  left: 0;
  top: 50%;
}

.slide-next-button {
  position: absolute;
  right: 0;
  top: 50%;
}

.img-size{
  width: 100%;
}

.top-page-title{
    position: absolute;
    color: rgb(156, 162, 49);
    font-size: 30px;
    top: 30%;
}
</style>
