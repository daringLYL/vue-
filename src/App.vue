<template>
<div class="back">
  <template class="header">
  <test_1 />
  </template>
  <div class="row">
  <test_2 />
  <test_3 />
  <test_4 />
  <test_5 />
  <test_6 />
  </div>
  <test_7 />
</div>
</template>

<script>
import test_1 from "./Test_1.vue"
import test_2 from "./Test_education.vue"
import test_3 from "./Test_language.vue"
import test_4 from "./Test_experience.vue"
import test_5 from "./Test_skills.vue"
import test_6 from "./Test_6.vue"
import test_7 from "./Test_7.vue"
export default{
  components:{ test_1 , test_2 , test_3 , test_4 , test_5 , test_6 , test_7 },
  }
</script>

<style scoped>
  @import '~@/index.css';
  .header{margin-left: -.1px;margin-right: -.1px;overflow: hidden;}
  .row{column-count:2;padding: 30px 45px;}
  .back{background-color: #f6fff6;width: 1030px;box-shadow: 3px 3px 9px rgba(0,0,0,.2);margin-top: 10px;margin-right: auto;margin-left: auto;}
</style>
