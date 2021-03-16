<template>
  <div class="box">
    <h2>Count is: {{ count }}</h2>
    <button @click="fetchData">Request Data</button>
    <button @click="clearData">Clear Data</button>
  </div>
</template>

<script>
const axios = require("axios");

export default {
  data() {
    return { count: 0 };
  },
  methods: {
    fetchData() {
      // Make a request for a user with a given ID
      axios
        .get("https://dog.ceo/api/breeds/list/all")
        .then(function (response) {
          // handle success
          console.log(response.data.message);
        })
        .catch(function (error) {
          // handle error
          console.log(error);
        })
        .then(function () {
          // always executed
        });
    },
    clearData() {},
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
.box button {
  margin-right: 10px;
}
</style>
