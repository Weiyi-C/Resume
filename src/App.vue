<template>
  <div>
    <Navbar />
    <router-view/>
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'
export default {
  name: 'App',
  data () {
    return {
      nav: [
        { name: '返回首页', url: '' },
        { name: '基本信息', url: '' },
        { name: 'Web', url: '' },
        { name: '移动', url: '' },
        { name: '设计', url: '' }
      ]
    }
  },
  components: {
    Navbar,
    Footer
  }
}
</script>

<style>

</style>
