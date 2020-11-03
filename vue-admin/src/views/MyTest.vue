<template>
  <div class="mymy">
    <img alt="Vue logo" src="../assets/logo.png" />
    <MyTestComponent msg="Welcome to Your Vue.js App 1111" />
    <MyTestComponent2 msg="conponent 2" />
  </div>
</template>

<script>
// @ is an alias to /src
import MyTestComponent from "@/components/MyTestComponent.vue";

export default {
  name: "MyTest1",
  components: {
    MyTestComponent,
    MyTestComponent2: () => import("@/components/MyTestComponent2.vue")
  }
};
</script>

<style>
#mymy {
  /* font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #30502c;
  margin-top: 610px; */
}
</style>
