<template>
  <button
    class="simple-button"
    v-bind:class="{
      neutral: isNeutral,
      alert: isAlert
    }"
  >
    {{ msg }}
  </button>
</template>

<script>
export default {
  name: 'Button',
  props: {
    msg: String,
    isAlert: Boolean,
    isNeutral: Boolean
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  .simple-button {
    display: block;
    font-family: "Roboto";
    line-height: 24px;
    border-radius: 50px;
    color: #FFF;
    max-width: 250px;
    width: 80vw;
    border: none;
  }
  .neutral {
    background-color: #48B9A8;
    font-size: 24px;
    padding: 24px;
  }
  .alert {
    background-color: #FC6C8C;
    font-size: 18px;
    padding: 12px;
  }

</style>
