<template>
  <div>
    <div class="button">
      <button @click="showReactContainer = !showReactContainer">Press me</button>
    </div>
    <div v-show="showReactContainer">
      <iframe id="root" src="/threekit.html" frameborder="0"></iframe>
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
    width:  100%;
  }

  .button {
    height: 50px;
    display: flex;
    justify-content: center;
    padding:  8px;
  }
</style>
