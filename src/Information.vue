<template>
  <dd :class="typeClass">
  {{type}}
  </dd>
</template>

<script>
export default {
  props: ["type", "typeClass"]
};
</script>

<style>
</style>
