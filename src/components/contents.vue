<template lang="pug">
.right-block-content
   .content-space
     .content-day
       span.gauzy TODAY
     .content-text
        span.accepted {{firstComment.comment}}
        p.time {{firstComment.time}}
     .content-text
       span.comment {{secondComment.comment}}
       p.time {{secondComment.time}}
     .comment-next
       span.comment-next-words {{thirdComment.comment}}
     .content-text
       span.uploads {{forthComment.comment}}
       p.time {{forthComment.time}}
     .photos
        img( v-for="(images, index) in ImagesNature" :src="images.image" :key="index" @click="setAtribute(index)")
     .counter {{ notification }}
</template>

<script lang="ts">
import img1 from './../assets/img/img1.png'
import img2 from './../assets/img/img2.png'
import img3 from './../assets/img/img3.png'
import img4 from './../assets/img/img4.png'
export default {
  name: 'contents',
  data () {
    return {
      notification: 3,
      firstComment: {
        comment: 'Darika Samak mark as done Listing on Product Hunt so that we can reach as many potential users',
        time: '8:40 PM'
      },
      secondComment: {
        comment: 'Emilee Simchenko commented on Account for teams and personal in bottom style',
        time: '7:32 PM'
      },
      thirdComment: {
        comment: 'During a project build, it is necessary to evaluate the product design and development against project requirements and outcomes'
      },
      forthComment: {
        comment: 'Darika Samak uploaded 4 files on An option to search in current projects or in all projects',
        time: '6:42 PM'
      },
      ImagesNature: [
        { image: img1 },
        { image: img2 },
        { image: img3 },
        { image: img4 }
      ]
    }
  },
  methods: {
    setAtribute (index:number) {
      console.log(index + 1) // this.notification = index
    }
  }
}
</script>

<style scoped>

</style>
