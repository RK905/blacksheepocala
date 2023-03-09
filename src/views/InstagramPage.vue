<template>
  <div>
    <h1>Latest post from @blacksheeponbroadway</h1>
    <iframe
      src="https://www.instagram.com/blacksheeponbroadway/embed/"
      width="100%"
      height="800"
      frameborder="0"
      scrolling="no"
      allowtransparency="true"
    ></iframe>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  components: {},
})
export default class InstagramPage extends Vue {}
</script>
