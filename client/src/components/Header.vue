<template>
  <Header>
    <img :src="image" />
  </Header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      image: require("@/assests/logo.png")
    };
  }
};
</script>

<style></style>
