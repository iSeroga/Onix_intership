<template lang="pug">
div
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
</template>

<script>
export default {
  name: 'headerBar'
}
</script>

<style scoped>

</style>
