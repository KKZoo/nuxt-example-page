<template>
  <section>
    <navbar />
    <topPage />
    <myprofPage />
    <skillPage />
  </section>
</template>

<script>
import navbar from '~/components/navbar.vue'
import topPage from '~/components/topPage.vue'
import myprofPage from '~/components/myprofPage.vue'
import skillPage from '~/components/skillPage.vue'

export default {
    components: {
        navbar,
        topPage,
        myprofPage,
        skillPage
    }      
}
</script>>