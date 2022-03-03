<template>
  <section class="container">
    <form action="login" method="GET">
      <div>
        姓名:<input type="text" name="name" required/>
      </div>
      <div>
        帳號:<input type="text" name="uid" required/>
      </div>
      <input type="submit"/>
    </form>
  </section>
</template>

<script>
export default {
  data: {
    hello: "hello world",
  },
  name: "IndexPage",
};
</script>
