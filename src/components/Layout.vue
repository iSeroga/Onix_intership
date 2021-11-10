<template lang="pug">
.first-block
  nav-bar
  header-bar

</template>

<script>
import navBar from './navBar'
import headerBar from './headerBar'

export default {
  name: 'Layout',
  components: {
    navBar,
    headerBar
  }
}
</script>

<style scoped>

</style>
