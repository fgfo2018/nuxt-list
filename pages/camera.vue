<template>
  <div id="c-item">
    <ul>
      <li v-for="(item, index) in info" :key="index">{{ item }}</li>
    </ul>
  </div>
</template>

<script>
import axios from "axios";
export default {
  name: "CameraPage",
//   data() {
//     return {
//       member: data1,
//     };
//   },
};
axios
  .get("http://192.168.0.173:8080/camera")
  .then(function (response) {
    var data = response.data;
    // data1 = ["Adam", "Jack", "Candy", "Louis", "Lurry"];
    console.log(data);
    return { info: response.data};
  })
  .catch(function (error) {
    console.log(error);
  });


</script>

<style>
</style>