<template>
  <div>
    <button @click="beforeSlide">
      前
    </button>
    <button @click="nextSlide">
      次
    </button>
    <transition name="slide">
      <div :key="products[product]">
        <img :src="products[product]" class="img-size">
      </div>
    </transition>
  </div>
</template>>

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
</script>>

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

.img-size{
  position: absolute;
  width: 100%;
}
</style>
