<template>
<dd :class="textClass">
  {{text}}
</dd>
</template>

<script>
export default {
  props: ["text", "textClass"]
};
</script>

<style>
</style>
