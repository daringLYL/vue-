<template>
   <li class="language-desc-item">
       {{text1}}
        <strong>{{pointText1}}</strong>{{text2}}
        <strong>{{pointText2}}</strong>{{text3}}
      </li>
</template>

<script>
export default {
  props: ["text1", "text2", "text3", "pointText1", "pointText2"]
};
</script>

<style>
</style>
