<template>
  <div>
    <section class="education">
      <plateTitle :title1="commonData.title[11]" :title2="commonData.title[12]" />
    </section>
    <educationPart
      :toTime="educationData.toTime[0]"
      :endTime="educationData.endTime[0]"
      :subject="educationData.subject[0]"
      :degree="educationData.degree[0]"
      :credit="educationData.credit[0]"
      :highScore="educationData.highScore[0]"
      :toHighScore="educationData.highScore[1]"
      :school="educationData.school"
    />
    <educationPart
      :toTime="educationData.toTime[1]"
      :endTime="educationData.endTime[1]"
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
import educationPart from "./EducationPart.vue";
import plateTitle from "./PlateTitle";
import data from "./data.json";
export default {
  components: { educationPart, plateTitle },
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

