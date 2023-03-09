<template>
  <div class="home-page">
    <h1>Welcome to my PWA!</h1>
    <p>This is the homepage for my progressive web app.</p>
  </div>
</template>

<style>
.home-page {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100%;
}

.nav-bar {
  display: flex;
  justify-content: center;
  background-color: #f8f8f8;
  padding: 10px;
  margin-bottom: 20px;
}

.nav-bar ul {
  list-style: none;
  display: flex;
  margin: 0;
  padding: 0;
}

.nav-bar li {
  margin-right: 20px;
}

.nav-bar li:last-child {
  margin-right: 0;
}
</style>
<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  components: {},
})
export default class HomeView extends Vue {}
</script>
