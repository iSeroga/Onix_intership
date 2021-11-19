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
    //.counter(v-for="(index, idx1) in ImagesNature" :key="idx1") {{ notification }}
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
.ask
  .ask-content
    p
      | Are u sure u want to change number of tasks?
    input.YesB(type='button' value='Yes')
    input.NoB(type='button' value='No')
</template>

<script lang="ts">
import { defineComponent } from 'vue'
export default defineComponent({
  name: 'navBar',

  data () {
    return {
      name: 'Joan Gonzales'
    }
  },
  mounted () {
    const askWindow = document.querySelector('.ask')!
    const closedNumbDesktop = document.querySelector('.closed')!// 374
    const openTaskDesktop = document.querySelector('.openB')!// 72
    closedNumbDesktop.addEventListener('click', () => {
      askWindow.classList.toggle('open-window')
    })
    const yesBtn = document.querySelector('.YesB')!
    const noBtn = document.querySelector('.NoB')!
    let numberOpen = Number(openTaskDesktop.textContent)
    let numberClosed = Number(closedNumbDesktop.textContent)
    yesBtn.addEventListener('click', () => {
      if (numberOpen > 0) {
        numberOpen = numberOpen - 1
        numberClosed = +numberClosed + 1
        askWindow.classList.toggle('open-window')
      } else {
        askWindow.classList.toggle('open-window')
      }
      openTaskDesktop.innerHTML = String(numberOpen)
      closedNumbDesktop.innerHTML = String(numberClosed)
    })
    noBtn.addEventListener('click', () => {
      askWindow.classList.toggle('open-window')
    })
  }
})
</script>
<style scoped></style>
