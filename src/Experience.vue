<template>
  <section class="experience">
    <plateTitle :title1="commonData.title[15]" :title2="commonData.title[16]" />
    <div class="timeline-wrapper">
      <ul class="sec-content timeline">
        <li class="timeline-item experience-internship">
          <headtitle :experience1="commonData.experience[0]" :experience2="commonData.experience[1]" :shortLine1="commonData.shortLine[0]" :shortLine2="commonData.shortLine[1]"
          :experience3="commonData.experience[2]" :experienceToTime="commonData.experienceToTime[0]" :experienceEndTime="commonData.experienceEndTime[0]"
          :showLink1="commonData.showLink[0]" :showLink2="commonData.showLink[0]" />
          <dl class="experience-description timeline-content">
            <subtitle :title1="commonData.title[0]" />
            <information :type="commonData.type.typeList[0]" :typeClass="commonData.typeClass[0]" />
            <subtitle :title1="commonData.title[1]" />
            <information :type="commonData.type.typeList[1]" :typeClass="commonData.typeClass[0]" />
            <information :type="commonData.type.typeList[2]" :typeClass="commonData.typeClass[0]" />
            <information :type="commonData.type.typeList[3]" :typeClass="commonData.typeClass[0]" />
          </dl>
        </li>
        <li class="timeline-item experience-internship">
          <div>
          <headtitle :experience1="commonData.experience[3]" :experience3="commonData.experience[4]" :shortLine1="commonData.shortLine[0]" :shortLine2="commonData.shortLine[1]"
          :experienceToTime="commonData.experienceToTime[1]" :experienceEndTime="commonData.experienceEndTime[1]" :showLink1="commonData.showLink[0]" :showLink2="commonData.showLink[0]" />
          </div>
          <dl class="experience-description timeline-content">
            <subtitle :title1="commonData.title[2]" />
            <information :type="commonData.type.typeList[4]" :typeClass="commonData.typeClass[0]" />
            <information :type="commonData.type.typeList[5]" :typeClass="commonData.typeClass[0]" />
          </dl>
        </li>
        <li class="timeline-item experience-project">
          <headtitle :experience1="commonData.experience[5]" :experienceProjectLink1="commonData.experienceProjectLink[0]"
          :experienceProjectLink2="commonData.experienceProjectLink[1]" :experienceProject1="commonData.experienceProject[0]" 
          :experienceProject2="commonData.experienceProject[1]" :showLink1="commonData.showLink[1]" :showLink2="commonData.showLink[1]" />
          <dl class="experience-description timeline-content">
            <subtitle :title1="commonData.title[3]" :title2="commonData.title[4]" />
            <div v-for="(type,index) in commonData.type.forTypeList[0]" :key="index">
              <information :type="type" :typeClass="commonData.typeClass[0]" />
            </div>
          </dl>
        </li>
        <li class="timeline-item experience-project">
          <headtitle :experience1="commonData.experience[5]" :experienceProjectLink1="commonData.experienceProjectLink[2]"
          :experienceProject1="commonData.experienceProject[0]" :showLink1="commonData.showLink[1]" :showLink2="commonData.showLink[0]"/>
          <dl class="experience-description timeline-content">
            <subtitle :title1="commonData.title[3]" :title2="commonData.title[4]" :title3="commonData.title[5]" />
           <div v-for="(type,index) in commonData.type.forTypeList[1]" :key="index">
              <information :type="type" :typeClass="commonData.typeClass[0]" />
            </div>
          </dl>
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

