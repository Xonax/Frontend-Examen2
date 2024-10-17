<template>
  <div class="container pt-5">
    <div class="row">
      <div class="col-12">
        <h2>All het nieuws!</h2>
      </div>
    </div>
    <div class="row pt-5">
      <div class="col-md-3 col-sm-6" v-for="(news, index) in newsList" :key="index"  @click="goToDetail(news.id)" >
        <div class="nieuws-container">
          <img :src="require(`@/assets/${news.image}`)" :alt="news.titel" />
          <div class="background"></div>
          <div class="d-flex info flex-column h-100">
            <h5>{{ news.titel }}</h5>
            <p class="mt-auto">{{ news.date }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
h5 {
  font-size: 12px;
}
.info * {
    position: relative;
    z-index: 3;
    margin: 0
}

.info {
    padding: .4rem
}

.nieuws-container {
    margin-bottom: 1rem;
    position: relative;
    aspect-ratio: 1
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

<script>
import news from "@/assets/data/nieuws";

export default {
  data() {
    return {
      newsList: news,
    };
  },
  methods: {
    goToDetail(newsId) {
      this.$router.push({ name: 'NewsDetail', params: { id: newsId } });
    }
  }
};
</script>
