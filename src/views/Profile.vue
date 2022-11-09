<template>

  <div class="display: inline-block grid grid-cols-3 gap-4 place-items-center">
    <profileCard name="GungGing" :year="year" :faculty="faculty"></profileCard>
    <profileCard name="Phum" :year="year" :faculty="faculty"></profileCard>
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
  </div>
</template>

<script>
import profileCard from "../components/Profile.vue";
export default {
  data() {
    return {
      name: "Mim",
      year: 1,
      faculty: "Science",
    };
  },
  components: {
    profileCard,
  },
};
</script>

<style></style>
