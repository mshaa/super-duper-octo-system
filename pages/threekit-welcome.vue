<template>
  <div>
    <div class="button">
      <button @click="showReactContainer = !showReactContainer">Press me</button>
    </div>
    <div v-show="showReactContainer">
      <div id="root"></div>
      <script src="welcome_threekit-embed.js"></script>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showReactContainer: false
    }
  }
}
</script>

<style>
  #root {
    height: calc(100vh - 50px);
  }

  .button {
    height: 50px;
    display: flex;
    justify-content: center;
    padding:  8px;
  }
</style>
