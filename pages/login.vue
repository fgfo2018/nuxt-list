<template>
  <div>
    <a type="button" href="/">回上一頁</a>
  </div>
</template>
<script>
import axios from "axios";
export default {
  name: "loginPage",
};
axios
  .get("http://localhost:8080/camera")
  .then(function (response) {
    var data = response.data;
  
    console.log(data);
  })
  .catch(function (error) {
    console.log(error);
  });

</script>