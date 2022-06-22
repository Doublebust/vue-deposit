<template>
  <aside v-if="modalOpen">
    <button class="exit" @click="closeModal">X</button>
    <video src="../../assets/banana.mp4" muted loop autoplay></video>
  </aside>
</template>

<script>
  export default {
    props: {
      modalOpen: {
        type: Boolean,
        required: true
      }
    },
    methods: {
      closeModal() {
        this.$emit('closeModalEvent')
      }
    }
  }
</script>


<style scoped>
  aside {
    position: fixed;
    top: 0;
    background: black;
    width: 100vw;
    height: 100vh;
    z-index: 10000;
    display: flex;
    justify-content: center;
    align-content: center;
  }

  video {
    width: 60%;
  }

  .exit {
    position: absolute;
    top: 0;
    right: 0;
    margin: 10px 10px 0;
    color: white;
    background: none;
    border: none;
  }
</style>