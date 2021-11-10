<template lang="pug">
.right-block-content
   .content-space
     .content-day
       span.gauzy TODAY
     .content-text.time1
      span.accepted {{firstComment.comment}}
     .content-text.time2
       span.comment {{secondComment.comment}}
     .comment-next
       span.comment-next-words {{thirdComment.comment}}
     .content-text.time3
       span.uploads {{forthComment.comment}}
     .photos
</template>

<script lang="ts">
export default {
  name: 'contents',
  data () {
    return {
      firstComment: {
        icon: '',
        comment: 'Darika Samak mark as done Listing on Product Hunt so that we can reach as many potential users',
        time: ''
      },
      secondComment: {
        icon: '',
        comment: 'Emilee Simchenko commented on Account for teams and personal in bottom style',
        time: ''
      },
      thirdComment: {
        icon: '',
        comment: 'During a project build, it is necessary to evaluate the product design and development against project requirements and outcomes',
        time: ''
      },
      forthComment: {
        icon: '',
        comment: 'Darika Samak uploaded 4 files on An option to search in current projects or in all projects',
        time: ''
      }
    }
  }
}
</script>

<style scoped>

</style>
