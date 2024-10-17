<template>
    <div class="container pt-5" v-if="newsDetail">
      <div class="row">
        <div class="col-12 pb-4">
          <h2>{{ newsDetail.titel }}</h2>
        </div>
        <div class="col-md-5">
            <p>{{ newsDetail.content }}</p>
        </div>
        <div class="col-md-6 offset-md-1">
            <img class="w-100 object-fit-cover" :src="require(`@/assets/${newsDetail.image}`)" :alt="newsDetail.titel" />
        </div>
      </div>
    </div>
    <div v-else>
      <p>Loading...</p>
    </div>
  </template>
  <script>
  import news from "@/assets/data/nieuws";
  
  export default {
    data() {
      return {
        newsDetail: null,
      };
    },
    created() {
      this.fetchNewsDetail();
    },
    methods: {
      fetchNewsDetail() {
        const newsId = parseInt(this.$route.params.id); // Ensure newsId is parsed to an integer
        this.newsDetail = news.find(newsItem => newsItem.id === newsId);
      },
    },
  };
  </script>
  
  <style scoped>
  .info * {
      position: relative;
      z-index: 3;
      margin: 0;
  }
  
  .info {
      padding: .4rem;
  }
  
  .nieuws-container {
      margin-bottom: 1rem;
      position: relative;
      aspect-ratio: 1;
  }
  
  .background {
      background-color: black;
      position: absolute;
      top: 0;
      width: 100%;
      aspect-ratio: 1;
      opacity: .3;
      z-index: 2;
  }
  
  .nieuws-container img {
      position: absolute;
      object-fit: cover;
      aspect-ratio: 1;
      width: 100%;
      z-index: 1;
  }
  </style>
  