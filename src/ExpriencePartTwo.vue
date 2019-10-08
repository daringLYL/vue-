<template>
  <dd class="experience-task">
    <strong>{{pointType1}}</strong>{{type1}}
    <strong>{{pointType2}}</strong>{{type2}}
    <strong>{{pointType3}}</strong>{{type3}}
    <strong>{{pointType4}}</strong>{{type4}}
    <strong>{{pointType5}}</strong>{{type5}}
    <strong>{{pointType6}}</strong>{{type6}}
    <span class="spaceFix"></span>{{otherType1}}
    <span class="spaceFix"></span>{{otherType2}}
    <strong>{{pointType7}}</strong>{{type7}}
    <strong>{{pointType8}}</strong>{{type8}}
    <strong>{{pointType9}}</strong>
  </dd>
</template>

<script>
export default {
  props: ["pointType1", "pointType2", "pointType3", "pointType4", "pointType5", "pointType6",
    "pointType7", "pointType8","pointType9", "type1", "type2", "type3", "type4", "type5", "type6",
     "type7","type8", "otherType1", "otherType2"
  ]
};
</script>

<style>
</style>