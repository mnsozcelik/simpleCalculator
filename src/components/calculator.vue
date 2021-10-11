<template>
  <div class="calculator-bg row justify-content-center">
    <div class="calculator col-md-3 col-sm-6 col-8 border-0 rounded p-0">
      <div class="screen row m-0 pm-0">
        <calculate-screen></calculate-screen>
      </div>

      <div class="keyboard row m-0 pm-0" style="bottom: 0">
        <calculator-keyboard></calculator-keyboard>
      </div>
    </div>
  </div>
</template>

<script>
import calculateScreen from "./calculateScreen.vue";
import calculatorKeyboard from "./calculatorKeyboard.vue";
export default {
  components: { calculateScreen, calculatorKeyboard },
};
</script>

<style scoped>
.calculator-bg {
  background-color: rgb(60, 163, 177);
  position: fixed;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  overflow: auto;
}
.calculator {
  margin-top: 6.2%;
  margin-bottom: 7%;
  background-color: black;
  border-radius: 15px !important;
}
</style>