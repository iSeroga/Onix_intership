<!--suppress HtmlUnknownTarget -->
<template lang="pug">
.right-block
  .right-block-header
    .right-block-header-left
      label.title-name Website Redesign
      .title-menu
        button
    .capabilities
      .another-users
        .another-users-photo
        .another-users-photo
        .another-users-photo
      button.share-link Share
      button.chat
        span.chat-logo Chat
  #nav.right-block-second-header
    a#1.second-header-choose(href='#') Tasks
    a#2.second-header-choose(href='#') Kanban
    a#3.second-header-choose(href='#') Activity
    a#4.second-header-choose(href='#') Calendar
    a#5.second-header-choose(href='#') Files
  .right-block-fon
    Contents
</template>

<script lang="ts">
import Contents from './contents.vue'
export default {
  name: 'headerBar',
  components: { Contents },
  mounted () {
    const navItem = document.querySelectorAll('.second-header-choose')
    let activNavItem = document.querySelector('.second-header-choose.active')
    navItem.forEach(navitem => {
      navitem.addEventListener('click', function () {
        navitem.classList.add('active')
        if (activNavItem != null) {
          activNavItem.classList.remove('active')
        }
        activNavItem = navitem
      })
    })
  }
}
</script>

<style scoped></style>
