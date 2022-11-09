<template>
  <div class="display: inline-block">
    <div
      class="box-content h-42 w-62 p-4 border-4 shadow-xl rounded-lg md:box-content hover:border-dashed hover:bg-gradient-to-b from-blue-500 to-pink-500 hover:text-white transition duration-300 ease-in-out hover:scale-105"
    >
      <img
        src="../assets/image/download.jpg"
        alt="image"
        class="rounded-full"
      />
      <br />
      <div class="font-mono md:whitespace-pre">
        <div class="font-black text-xl flex justify-center">MY PROFILE</div>

        <div class="flex justify-center">{{ name }}</div>
        <div class="flex justify-center">Year {{ year }}</div>
        <div class="flex justify-center">Faculty of {{ faculty }}</div>
        <br />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    name: { type: String, default: "Polite Cat" },
    year: {
      type: Number,
      default: 1,
    },
    faculty: {
      type: String,
      default: "Polite",
    },
    image: {
      type: String,
      default: "../assets/image/download.jpg",
    },
  },
};
</script>
<style></style>
