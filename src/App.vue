<template>
  <div class="background-container" :style="backgroundStyle">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
export default {
  data() {
    return {
      backgroundUrl: require('@/assets/main_background_office.jpg')
    };
  },
  computed: {
    backgroundStyle() {
      return {
        backgroundImage: `url(${this.backgroundUrl})`,
        backgroundSize: 'cover',
        backgroundPosition: 'center'
      };
    }
  }
};
</script>

<style scoped>
.background-container {
  width: 100%;
  height: 400px;
}
</style>
