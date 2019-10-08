<template>
   <li class="language-desc-item">
       能够
        <strong>{{pointText1}}</strong>{{text1}}
        <strong>{{pointText2}}</strong>{{text2}}
      </li>
</template>

<script>
export default {
  props: ["text1", "text2", "pointText1", "pointText2"]
};
</script>

<style>
</style>