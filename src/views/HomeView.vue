<template>
  <div class="main">
    <textSlider />
    <LastNews />
  </div>
</template>

<script>

// @ is an alias to /src
import textSlider from "@/components/text-slider.vue"
import LastNews from "@/components/Last-News.vue"


export default {
  name: 'HomeView',
  components: {
    textSlider,
    LastNews
  }
}
</script>
