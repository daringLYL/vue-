<template>
  <section class="experience">
    <PlateTitle :title1="commonData.title.plateTitle[4]" :title2="commonData.title.plateTitle[5]" />
    <div class="timeline-wrapper">
      <ul class="sec-content timeline">
        <li class="timeline-item experience-internship">
          <Headtitle :headtitle1="commonData.title.headTitle[0]" :headtitle2="commonData.title.headTitle[1]" :shortLine1="commonData.shortLine[0]" :shortLine2="commonData.shortLine[1]"
          :headtitle3="commonData.title.headTitle[2]" :toTime="commonData.toTime[2]" :endTime="commonData.endTime[2]"
          :showLink1="commonData.onShow[0]" :showLink2="commonData.onShow[0]" />
          <dl class="experience-description timeline-content">
            <Subtitle :title1="commonData.title.subtitle[0]" />
            <Information :text="commonData.text.textList[3]" :textClass="commonData.textClass[0]" />
            <Subtitle :title1="commonData.title.subtitle[1]" />
            <Information :text="commonData.text.textList[4]" :textClass="commonData.textClass[0]" />
            <Information :text="commonData.text.textList[5]" :textClass="commonData.textClass[0]" />
            <Information :text="commonData.text.textList[6]" :textClass="commonData.textClass[0]" />
          </dl>
        </li>
        <li class="timeline-item experience-internship">
          <div>
          <Headtitle :headtitle1="commonData.title.headTitle[3]" :headtitle3="commonData.title.headTitle[4]" :shortLine1="commonData.shortLine[0]" :shortLine2="commonData.shortLine[1]"
          :toTime="commonData.toTime[3]" :endTime="commonData.endTime[3]" :showLink1="commonData.onShow[0]" :showLink2="commonData.onShow[0]" />
          </div>
          <dl class="experience-description timeline-content">
            <Subtitle :title1="commonData.title.subtitle[2]" />
            <Information :text="commonData.text.textList[7]" :textClass="commonData.textClass[0]" />
            <Information :text="commonData.text.textList[8]" :textClass="commonData.textClass[0]" />
          </dl>
        </li>
        <li class="timeline-item experience-project">
          <Headtitle :headtitle1="commonData.title.headTitle[5]" :projectLink1="commonData.projectLink[0]"
          :projectLink2="commonData.projectLink[1]" :project1="commonData.project[0]" 
          :project2="commonData.project[1]" :showLink1="commonData.onShow[1]" :showLink2="commonData.onShow[1]" />
          <dl class="experience-description timeline-content">
            <Subtitle :title1="commonData.title.subtitle[3]" :title2="commonData.title.subtitle[4]" />
            <div v-for="(text,index) in commonData.text.circulationText[0]" :key="index">
              <Information :text="text" :textClass="commonData.textClass[0]" />
              <!--工作經歷——個人項目——Project Minder-->
            </div>
          </dl>
        </li>
        <li class="timeline-item experience-project">
          <Headtitle :headtitle1="commonData.title.headTitle[5]" :projectLink1="commonData.projectLink[2]"
          :project1="commonData.project[0]" :showLink1="commonData.onShow[1]" :showLink2="commonData.onShow[0]"/>
          <dl class="experience-description timeline-content">
            <Subtitle :title1="commonData.title.subtitle[3]" :title2="commonData.title.subtitle[4]" :title3="commonData.title.subtitle[5]" />
           <div v-for="(text,index) in commonData.text.circulationText[1]" :key="index">
              <Information :text="text" :textClass="commonData.textClass[0]" />
              <!--工作經歷——個人項目——Project Minder Mobile-->
            </div>
          </dl>
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
