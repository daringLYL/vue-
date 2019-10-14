<template>
  <div>
    <section class="education">
      <PlateTitle :title1="commonData.title.plateTitle[0]" :title2="commonData.title.plateTitle[1]" />
    </section>
    <EducationPart
      :toTime="commonData.toTime[0]"
      :endTime="commonData.endTime[0]"
      :subject="educationData.subject[0]"
      :degree="educationData.degree[0]"
      :credit="educationData.credit[0]"
      :highScore="educationData.highScore[0]"
      :toHighScore="educationData.highScore[1]"
      :school="educationData.school"
    />
    <EducationPart
      :toTime="commonData.toTime[1]"
      :endTime="commonData.endTime[1]"
      :subject="educationData.subject[1]"
      :degree="educationData.degree[1]"
      :credit="educationData.credit[1]"
      :highScore="educationData.highScore[2]"
      :toHighScore="educationData.highScore[3]"
      :school="educationData.school"
    />
  </div>
</template>

<script>
import EducationPart from "./EducationPart.vue";
import PlateTitle from "./PlateTitle";
import data from "./data.json";
export default {
  components: { EducationPart, PlateTitle },
  data() {
    return {
      educationData: data.EducationData,
      commonData: data.CommonData
    };
  }
};
</script>

<style>
</style>
