<template>
<div class="back">
  <template class="header">
  <headerInfo />
  </template>
  <div class="row">
  <education />
  <language />
  <experience />
  <skills />
  <contact />
  </div>
  <footerInfo />
</div>
</template>

<script>
import headerInfo from "./HeaderInfo.vue"
import education from "./Education.vue"
import language from "./Language.vue"
import experience from "./Experience.vue"
import skills from "./Skills.vue"
import contact from "./Contact.vue"
import footerInfo from "./FooterInfo.vue"
export default{
  components:{ headerInfo , education , language , experience , skills , contact , footerInfo },
  }
</script>

<style scoped>
  @import '~@/index.css';
  .header{margin-left: -.1px;margin-right: -.1px;overflow: hidden;}
  .row{column-count:2;padding: 30px 45px;}
  .back{background-color: #f6fff6;width: 1030px;box-shadow: 3px 3px 9px rgba(0,0,0,.2);margin-top: 10px;margin-right: auto;margin-left: auto;}
</style>
