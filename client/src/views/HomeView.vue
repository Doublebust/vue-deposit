<template>
  <div v-if="pageData">
    <home-header :videoTitle="pageData.videoHeroTitle" :videoSubTitle="pageData.videoSubTitle" :videoButton="pageData.videoButton"></home-header>
    <home-about></home-about>
    <home-secondary></home-secondary>
    <home-icons></home-icons>
  </div>
</template>

<script>
  import axios from 'axios';
  import homeHeader from '@/components/home/homeHeader';
  import homeAbout from '@/components/home/homeAbout';
  import homeSecondary from '@/components/home/homeSecondary';
  import homeIcons from '@/components/home/homeIcons';
  export default {
    components: {
      homeHeader,
      homeAbout,
      homeSecondary,
      homeIcons,
    },
    data() {
      return {
        pageData: null
      }
    },
    created() {
      // When page is created do whatever is in here...
      this.getPageData();
    },
    methods: {
      async getPageData() {
        const { data } = await axios.get('http://localhost:1337/api/home');
        this.pageData = data.data.attributes;
      }
    }
  }
</script>

