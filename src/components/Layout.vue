<template>
  <div class="first-block">
    <nav-bar/>
    <header-bar/>
    <contents/>
  </div>
</template>

<script>
import navBar from './navBar'
import headerBar from './headerBar'
import Contents from './contents'
export default {
  name: 'Layout',
  components: {
    Contents,
    navBar,
    headerBar
  }
}
</script>

<style scoped>
.the_most_main{
  display: flex;
  flex-flow: column;
}

</style>
