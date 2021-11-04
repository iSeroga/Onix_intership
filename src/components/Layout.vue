<template>
  <div class="first-block">
    <nav-bar/>
    <header-bar/>
  </div>
</template>

<script>
import navBar from './navBar'
import headerBar from './headerBar'

export default {
  name: 'Layout',
  components: {
    navBar,
    headerBar
  },
  data(){
    return{

    }
  },
  methods:{

  },
  mounted() {

  }
}
</script>

<style scoped>

</style>
