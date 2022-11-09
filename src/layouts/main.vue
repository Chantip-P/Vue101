<template>
  <div>
    <div
      class="font-black text-5xl flex justify-around box-content h-36 content-around h-14 bg-gradient-to-r from-blue-500 to-pink-500 text-white"
    >
      <br />
      ReanX2
      <br />
    </div>
    <div>
      <br>
      <nav class="flex space-x-10 flex justify-center text-2xl">
        <RouterLink to="/" class="hover:text-pink-500">Home</RouterLink>

        <RouterLink class="hover:text-pink-500" to="/about">About</RouterLink>

        <RouterLink class="hover:text-pink-500" to="/profile"
          >Profile</RouterLink
        >
      </nav>
      <br>
    </div>
    <slot></slot>
  </div>
</template>

<script>
export default {};
</script>

<style></style>
