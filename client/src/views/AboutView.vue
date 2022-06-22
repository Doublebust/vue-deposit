<template>
  <div>
    <about-header></about-header>
    <about-intro></about-intro> 
    <about-row></about-row> 
    <button @click="triggerModal">OPEN MODAL</button>
    <video-overlay :modalOpen="jaidPoop" @closeModalEvent="triggerModal" />
  </div>
</template>

<script>
  import aboutHeader from '@/components/about/aboutHeader';
  import aboutIntro from '@/components/about/aboutIntro';
  import aboutRow from '@/components/about/aboutRow';
  import videoOverlay from '@/components/global/videoOverlay'

  export default {
    data() {
      return {
        jaidPoop: false
      }
    },
    methods: {
      triggerModal() {
        this.jaidPoop = !this.jaidPoop;
      },
    },
    components: {
      aboutHeader,
      aboutIntro,
      aboutRow,
      videoOverlay
    }
  }
</script>