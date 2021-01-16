<template>
  <div>Index</div>
</template>

<script lang="ts">
import { defineComponent, useContext } from "@nuxtjs/composition-api";

export default defineComponent({
  setup() {
    const context = useContext()

    // $axios instance
    context.$axios.get('/')

    // router instance
    context.store.$router.push('/')
  }
});
</script>
