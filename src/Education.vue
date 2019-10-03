<template>
  <div>
    <section class="education">
      <div class="sec-title-wrapper">
        <h3 class="sec-title">
          <span class="sec-title-ch">教育经历</span>
          <span class="sec-title-en">Education</span>
        </h3>
      </div>
    </section>
    <educationPart toTime="2015" endTime="2016" subject="数据科学" degree="硕士" credit="5.91" outstandingSub="移动网络工程，学术研究实践" 
    toOutstangdingSub="普适移动系统开发，毕业设计项目1，2"/>
    <educationPart toTime="2012" endTime="2014" subject="信息科技" degree="学士" credit="5.44" outstandingSub="电子商业网站开发，网页设计与开发"
    toOutstangdingSub="数据库设计，游戏产业入门"/>
  </div>
</template>

<script>
import educationPart from "./EducationPart.vue"
export default {components:{ educationPart } };
</script>

<style>
</style>
