<template>
  <div class="container keyboard">
    <div class="row">
      <div class="col clcBtn" @click="clear">
        <span class="clcBtnTxt">C</span>
      </div>
      <div class="col clcBtn" @click="del">
        <span class="clcBtnTxt">D</span>
      </div>
      <div class="col clcBtn" @click="add('%')">
        <span class="clcBtnTxt">%</span>
      </div>
      <div class="col clcBtn" @click="add('%')">
        <span class="clcBtnTxt">+</span>
      </div>
    </div>
    <div class="row">
      <div class="col clcBtn" @click="add('1')">
        <span class="clcBtnTxt">1</span>
      </div>
      <div class="col clcBtn" @click="add('2')">
        <span class="clcBtnTxt">2</span>
      </div>
      <div class="col clcBtn" @click="add('3')">
        <span class="clcBtnTxt">3</span>
      </div>
      <div class="col clcBtn" @click="add('-')">
        <span class="clcBtnTxt">-</span>
      </div>
    </div>
    <div class="row">
      <div class="col clcBtn" @click="add('4')">
        <span class="clcBtnTxt">4</span>
      </div>
      <div class="col clcBtn" @click="add('5')">
        <span class="clcBtnTxt">5</span>
      </div>
      <div class="col clcBtn" @click="add('6')">
        <span class="clcBtnTxt">6</span>
      </div>
      <div class="col clcBtn" @click="add('*')">
        <span class="clcBtnTxt">x</span>
      </div>
    </div>
    <div class="row">
      <div class="col clcBtn" @click="add('7')">
        <span class="clcBtnTxt">7</span>
      </div>
      <div class="col clcBtn" @click="add('8')">
        <span class="clcBtnTxt">8</span>
      </div>
      <div class="col clcBtn" @click="add('9')">
        <span class="clcBtnTxt">9</span>
      </div>
      <div class="col clcBtn" @click="add('/')">
        <span class="clcBtnTxt">/</span>
      </div>
    </div>

    <div class="row">
      <div
        class="col-3 clcBtn"
        @click="add('0')"
        style="border-radius: 0 0 0 15px !important"
      >
        <span class="clcBtnTxt">0</span>
      </div>
      <div class="col-3 clcBtn" @click="add('.')">
        <span class="clcBtnTxt">.</span>
      </div>
      <div
        class="col-6 clcBtn"
        @click="equal"
        style="border-radius: 0 0 15px 0 !important"
      >
        <span class="clcBtnTxt">=</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  methods: {
    clear() {
      alert("temizle");
    },
    del() {
      alert("sondakini sil");
    },
    equal() {},
  },
};
</script>

<style scoped>
.keyboard {
  background-image: linear-gradient(to right, rgb(0, 0, 0), rgb(60, 163, 177));
  padding: 0px;
  border-radius: 0 0 15px 15px !important;
}
.row {
  width: 100%;
  padding: 0;
  margin: 0;
}
.clcBtn {
  cursor: pointer;
  background-color: rgba(0, 0, 0, 0.233);
  border: 2px solid rgba(0, 0, 0, 0.116);
  height: 65px;
}
.clcBtn:hover {
  background-color: rgba(83, 83, 83, 0.452);
}

.clcFuncButton {
}
.clcBtnTxt {
  color: whitesmoke;
  font-size: 28px;
  font-weight: bold;
  display: table;
  margin: auto;
}
</style>