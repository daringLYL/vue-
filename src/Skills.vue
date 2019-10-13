<template>
  <section class="skills">
    <plateTitle :title1="commonData.title[17]" :title2="commonData.title[18]" />
    <div class="timeline-wrapper">
      <ul class="sec-content timeline">
        <li class="timeline-item skills-frontend">
          <headtitle :experience1="commonData.experience[6]" :experience2="commonData.experience[7]" />
          <dl class="skills-description timeline-content">
            <subtitle :title1="commonData.title[6]" />
            <information :type="commonData.type.typeList[6]" :typeClass="commonData.typeClass[1]" />
            <information :type="commonData.type.typeList[7]" :typeClass="commonData.typeClass[1]" />
            <subtitle :title1="commonData.title[7]" />
            <information :type="commonData.type.typeList[8]" :typeClass="commonData.typeClass[1]" />
            <subtitle :title1="commonData.title[8]" />
            <information :type="commonData.type.typeList[9]" :typeClass="commonData.typeClass[1]" />
            <subtitle :title1="commonData.title[9]" />
            <div v-for="(type,index) in commonData.type.forTypeList[2]" :key="index">
              <information :type="type" :typeClass="commonData.typeClass[1]" />
            </div>
          </dl>
        </li>
        <li class="timeline-item skills-backend">
         <headtitle :experience1="commonData.experience[6]" :experience2="commonData.experience[8]" />
          <dl class="skills-description timeline-content">
            <subtitle :title1="commonData.title[10]" />
            <information :type="commonData.type.typeList[10]" :typeClass="commonData.typeClass[1]" />
            <information :type="commonData.type.typeList[11]" :typeClass="commonData.typeClass[1]" />
            <information :type="commonData.type.typeList[12]" :typeClass="commonData.typeClass[1]" />
          </dl>
        </li>
        <li class="timeline-item skills-miscellaneous">
          <headtitle :experience1="commonData.experience[9]" />
          <ul class="skills-description skills-miscellaneous timeline-content">
            <div v-for="(type,index) in commonData.type.forTypeList[3]" :key="index">
              <information :type="type" :typeClass="commonData.typeClass[1]" />
            </div>
          </ul>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
import headtitle from "./Headtitle.vue"
import subtitle from "./Subtitle.vue"
import information from "./Information.vue"
import plateTitle from "./PlateTitle"
import data from "./data.json"
export default {
   components: { headtitle, subtitle, information, plateTitle },
   data() {
    return {
      commonData: data.CommonData
    }
}};
</script>

<style>
</style>
