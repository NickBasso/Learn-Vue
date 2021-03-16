<template>
  <div class="box">
    <h2>Count is: {{ count }}</h2>
    <button @click="count += 1">Increment</button>
    <button @click="count = 0">Reset</button>
  </div>
</template>

<script>
export default {
  data() {
    return { count: 0 };
  },
};
</script>

<style>
.box {
  background: #e3e3e3;
  padding: 10px;
  margin: 10px;
  border: 1px solid #c5c5c5;
}
</style>
