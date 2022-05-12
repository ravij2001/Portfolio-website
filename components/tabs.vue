<template>
  <div class="bg-gray-800 text-center text-white my-5 tabc">
    <span
      class="tab"
      v-for="(tab, index) in tabs"
      :key="index"
      :class="{ activeTab: selectedTab === tab }"
      @click="selectedTab = tab"
      >{{ tab }}</span
    >
    <div
      v-show="selectedTab === 'All Works'"
      class="grid grid-cols-3 gap-3 my-5 container"
    >
      <img
        :src="i1"
        style="height: 300px; width: 350px"
        class="
          m-3
          transition
          duration-500
          ease-in-out
          bg-blue-600
          hover:bg-red-600
          transform
          hover:-translate-y-1 hover:scale-110
        "
      />
      <img
        :src="i2"
        style="height: 300px; width: 350px"
        class="
          m-3
          transition
          duration-500
          ease-in-out
          bg-blue-600
          hover:bg-red-600
          transform
          hover:-translate-y-1 hover:scale-110
        "
      />
      <img
        :src="i3"
        style="height: 300px; width: 350px"
        class="
          m-3
          transition
          duration-500
          ease-in-out
          bg-blue-600
          hover:bg-red-600
          transform
          hover:-translate-y-1 hover:scale-110
        "
      />
      <br />
      <img
        :src="i4"
        style="height: 300px; width: 350px"
        class="
          m-3
          transition
          duration-500
          ease-in-out
          bg-blue-600
          hover:bg-red-600
          transform
          hover:-translate-y-1 hover:scale-110
        "
      />
      <img
        :src="i5"
        style="height: 300px; width: 350px"
        class="
          m-3
          transition
          duration-500
          ease-in-out
          bg-blue-600
          hover:bg-red-600
          transform
          hover:-translate-y-1 hover:scale-110
        "
      />
    </div>

    <div
      v-show="selectedTab === 'Art Directions'"
      class="grid grid-cols-3 gap-3 my-5 container"
    >
      <img
        :src="i1"
        style="height: 300px; width: 350px"
        class="
          m-3
          transition
          duration-500
          ease-in-out
          bg-blue-600
          hover:bg-red-600
          transform
          hover:-translate-y-1 hover:scale-110
        "
      />
      <img
        :src="i2"
        style="height: 300px; width: 350px"
        class="
          m-3
          transition
          duration-500
          ease-in-out
          bg-blue-600
          hover:bg-red-600
          transform
          hover:-translate-y-1 hover:scale-110
        "
      />
    </div>

    <div
      v-show="selectedTab === 'Branding'"
      class="grid grid-cols-3 gap-3 my-5 container"
    >
      <img
        :src="i2"
        style="height: 300px; width: 350px"
        class="
          m-3
          transition
          duration-500
          ease-in-out
          bg-blue-600
          hover:bg-red-600
          transform
          hover:-translate-y-1 hover:scale-110
        "
      />
      <img
        :src="i3"
        style="height: 300px; width: 350px"
        class="
          m-3
          transition
          duration-500
          ease-in-out
          bg-blue-600
          hover:bg-red-600
          transform
          hover:-translate-y-1 hover:scale-110
        "
      />
    </div>

    <div
      v-show="selectedTab === 'Design'"
      class="grid grid-cols-3 gap-3 my-5 container"
    >
      <img
        :src="i4"
        style="height: 300px; width: 350px"
        class="
          m-3
          transition
          duration-500
          ease-in-out
          bg-blue-600
          hover:bg-red-600
          transform
          hover:-translate-y-1 hover:scale-110
        "
      />
      <img
        :src="i5"
        style="height: 300px; width: 350px"
        class="
          m-3
          transition
          duration-500
          ease-in-out
          bg-blue-600
          hover:bg-red-600
          transform
          hover:-translate-y-1 hover:scale-110
        "
      />
    </div>

    <div
      v-show="selectedTab === 'Web'"
      class="grid grid-cols-3 gap-3 my-5 container"
    >
      <img
        :src="i3"
        style="height: 300px; width: 350px"
        class="
          m-3
          transition
          duration-500
          ease-in-out
          bg-blue-600
          hover:bg-red-600
          transform
          hover:-translate-y-1 hover:scale-110
        "
      />
      <img
        :src="i2"
        style="height: 300px; width: 350px"
        class="
          m-3
          transition
          duration-500
          ease-in-out
          bg-blue-600
          hover:bg-red-600
          transform
          hover:-translate-y-1 hover:scale-110
        "
      />
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      tabs: ["All Works", "Art Directions", "Branding", "Design", "Web"],
      selectedTab: "All Works",
      i1: "i1.jpg",
      i2: "i2.jpg",
      i3: "i3.jpg",
      i4: "i4.jpg",
      i5: "i5.jpg",
      i6: "i6.jpg",
    };
  },
};
</script>
<style scoped>
.tab {
  margin-left: 30px;
  cursor: pointer;
  padding: 10px;
}
.tab:hover {
  background-color: red;
  border: 2px solid red;
  color: white;
  border-radius: 20px;
}
.tabc {
  height: 800px;
}
.activeTab {
  border: 2px solid red;
  color: white;
  border-radius: 20px;
  padding: 10px;
  text-decoration: none;
}
.activeTab:hover {
  background-color: red;
}
</style>