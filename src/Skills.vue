<template>
  <section class="skills">
    <PlateTitle :title1="commonData.title.plateTitle[6]" :title2="commonData.title.plateTitle[7]" />
    <div class="timeline-wrapper">
      <ul class="sec-content timeline">
        <li class="timeline-item skills-frontend">
          <Headtitle :headtitle1="commonData.title.headTitle[6]" :headtitle2="commonData.title.headTitle[7]" />
          <dl class="skills-description timeline-content">
            <Subtitle :title1="commonData.title.subtitle[6]" />
            <Information :text="commonData.text.textList[9]" :textClass="commonData.textClass[1]" />
            <Information :text="commonData.text.textList[10]" :textClass="commonData.textClass[1]" />
            <Subtitle :title1="commonData.title.subtitle[7]" />
            <Information :text="commonData.text.textList[11]" :textClass="commonData.textClass[1]" />
            <Subtitle :title1="commonData.title.subtitle[8]" />
            <Information :text="commonData.text.textList[12]" :textClass="commonData.textClass[1]" />
            <Subtitle :title1="commonData.title.subtitle[9]" />
            <div v-for="(text,index) in commonData.text.circulationText[2]" :key="index">
              <Information :text="text" :textClass="commonData.textClass[1]" />
              <!--技能——Web 前端——前端工程实践-->
            </div>
          </dl>
        </li>
        <li class="timeline-item skills-backend">
         <Headtitle :headtitle1="commonData.title.headTitle[6]" :headtitle2="commonData.title.headTitle[8]" />
          <dl class="skills-description timeline-content">
            <Subtitle :title1="commonData.title.subtitle[10]" />
            <Information :text="commonData.text.textList[13]" :textClass="commonData.textClass[1]" />
            <Information :text="commonData.text.textList[14]" :textClass="commonData.textClass[1]" />
            <Information :text="commonData.text.textList[15]" :textClass="commonData.textClass[1]" />
          </dl>
        </li>
        <li class="timeline-item skills-miscellaneous">
          <Headtitle :headtitle1="commonData.title.headTitle[9]" />
          <ul class="skills-description skills-miscellaneous timeline-content">
            <div v-for="(text,index) in commonData.text.circulationText[3]" :key="index">
              <Information :text="text" :textClass="commonData.textClass[1]" />
              <!--技能——其他-->
            </div>
          </ul>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
import Headtitle from "./Headtitle.vue"
import Subtitle from "./Subtitle.vue"
import Information from "./Information.vue"
import PlateTitle from "./PlateTitle"
import data from "./data.json"
export default {
   components: { Headtitle, Subtitle, Information, PlateTitle },
   data() {
    return {
      commonData: data.CommonData
    }
}};
</script>

<style>
</style>
