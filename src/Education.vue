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
    <educationPart
      :toTime="educationData.toTime1"
      :endTime="educationData.endTime1"
      :subject="educationData.subject1"
      :degree="educationData.degree1"
      :credit="educationData.credit1"
      :outstandingSub="educationData.outstandingSub1"
      :outstandingSub2="educationData.outstandingSub2"
    />
    <educationPart
      :toTime="educationData.toTime2"
      :endTime="educationData.endTime2"
      :subject="educationData.subject2"
      :degree="educationData.degree2"
      :credit="educationData.credit2"
      :outstandingSub="educationData.outstandingSub3"
      :outstandingSub2="educationData.outstandingSub4"
    />
  </div>
</template>

<script>
import educationPart from "./EducationPart.vue";
import data from "./data.json";
export default {
  components: { educationPart },
  mounted() {
    console.log(this.educationData);
  },
  data() {
    return {
      educationData: data
    };
  }
};
</script>

<style>
</style>
