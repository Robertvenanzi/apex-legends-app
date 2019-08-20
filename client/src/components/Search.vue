<template>
  <section class="search">
    <h1>Track Player Stats</h1>
    <form v-on:onsubmit.prevent="onSubmit">
      <div class="form-group">
        <label for="platform">Platform</label>
        <select name="platform" id="platform" v-modal="platform">
          <option value="psn">Playstation</option>
          <option value="xbl">Xbox</option>
          <option value="origin">Origin</option>
        </select>
      </div>
      <div class="form-group">
        <label for="gamertag">gamertag</label>
        <input
          type="text"
          name="text"
          v-model="gamertag"
          id="gamertag"
          placeholder="Origin ID, Xbox Live ID, PSN ID, etc"
        />
      </div>
      <div class="form-group">
        <input type="submit" value="Submit" class="btn" />
      </div>
    </form>
  </section>
</template>

<script>
export default {
  name: "Search",
  data() {
    return {
      platform: "psn",
      gamertag: ""
    };
  },
  beforeCreate() {
    document.body.className = "body-bg-image";
  }
};
</script>

<style></style>
