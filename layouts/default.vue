<template>
  <div>
    <Header />
    <TitleArea />
    <nuxt />
    <Footer />
  </div>
</template>
<script>
import Header from  '~/layouts/common/Header.vue'
import Footer from  '~/layouts/common/Footer.vue'
import TitleArea from '~/components/TitleArea.vue'
export default {
  components:{
    Header,
    Footer,
    TitleArea

  }
}
</script>
