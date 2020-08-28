<template>
  <section>
    <navbar />
    <topPage />
    <skillPage />
  </section>
</template>

<script>
import navbar from '~/components/navbar.vue'
import topPage from '~/components/topPage.vue'
import skillPage from '~/components/skillPage.vue'

export default {
    components: {
        navbar,
        topPage,
        skillPage
    }      
}
</script>>