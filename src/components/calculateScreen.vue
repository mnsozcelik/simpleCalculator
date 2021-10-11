<template>
  <div class="border-0 rounded col-12 p-2">
    <h2 class="transaction">{{ transaction }}</h2>
    <h1 class="result">{{ result }}</h1>
  </div>
</template>

<script>
export default {
  data() {
    return {
      transaction: "200 + 59",
      result: 259,
    };
  },
};
</script>

<style>
.result,
.transaction {
  direction: rtl;
  caret-color: rgb(6, 2, 243);
  color: whitesmoke;
}
.result {
  margin-right: 6px;
}
.form-control:focus {
  border-color: #ff000000;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0), 0 0 8px rgba(255, 0, 0, 0);
}
</style>