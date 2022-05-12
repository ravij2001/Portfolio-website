<template>
  <div class="myservices text-center bg-gray-800">
    <p class="text-red-600 text-3xl">{{About}}</p>
    <h1 class="text-7xl text-white my-5">{{services}}</h1>
    <p class="text text-white">
      {{pWord}}
    </p>
  </div>
</template>
<script>
export default {
  props: {
    About: {
      type: String,
      default: "",
    },
    services: {
      type: String,
      default: "",
    },
    pWord: {
      type: String,
      default: "",
    },
  },
};
</script>
