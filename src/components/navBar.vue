<!--suppress ALL -->
<template lang="pug">
.left-block
  .left-block-header
    span.site-name PROJECTUS
  .left-block-user
    .user-photo
    .user
      span.name {{this.name}}
      br
      span.work.gauzy Product Owner
    .user-menu
      label.menu
        button
  .left-block-stats
    .complete
      strong.closed 372
      br
      span.gauzy Completed Tasks
    .open
      strong.openB 11
      br
      span.gauzy Open Tasks
  .left-block-menu
    p.gauzy MENU
    br
    p Home
    br
    p My Tasks
    br
    p.message Notifications
    .counter
  //.left-block2
  //  .mobile-menu
  //    .user-photo
  //    .user
  //      span.name Jean Gonzales
  //      br
  //      span.work.gauzy Product Owner
  //    .left-block-stats
  //      .complete
  //        p.closed 372
  //        span.gauzy Completed Tasks
  //      .open
  //        p.openB 11
  //        span.gauzy Open Tasks
  //    .left-block-menu
  //      p.gauzy MENU
  //      br
  //      p Home
  //      br
  //      p My Tasks
  //      br
  //      p.message Notifications
  //      .counter
  //      br
  //  .left-block2-header
  //    label#hiddenMenu.hidden-menu(for='reveal')
  //      img(src='../assets/img/dwegalochki.svg' alt='dwegalochki')
  //      input#reveal(type='button' value='Hidden-menu')
  //    span.site-name2 PROJECTUS
</template>

<script lang="ts">
export default {
  name: 'navBar',
  data(){
    return{
      name:'Joan Gonzales'
    }
  }
}
</script>

<style scoped></style>
