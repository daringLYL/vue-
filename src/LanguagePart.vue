<template>
  <div class="language-cert-wrapper">
    <dt class="language-cert-type">{{language}}</dt>
    <dd class="progress language-cert-score">
      <div :style="width" class="progress-bar">
        <span class="progress-label">{{level}}</span>
      </div>
    </dd>
  </div>
</template>

<script>
export default {
  props: ["language", "level", "width"]
};
</script>

<style>
</style>
