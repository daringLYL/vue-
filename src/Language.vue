<template>
  <section class="language">
    <plateTitle :title1="commonData.title[13]" :title2="commonData.title[14]" />
    <div class="sec-content">
      <dl class="language-certificates">
        <languagePart :language="languageData.language[0]" :level="languageData.level[0]" :width="languageData.width[0]" />
        <languagePart :language="languageData.language[1]" :level="languageData.level[1]" :width="languageData.width[1]" />
        <languagePart :language="languageData.language[2]" :level="languageData.level[2]" :width="languageData.width[2]" />
      </dl>
    </div>
    <ul class="language-description">
      <languagePartTwo :text1="languageData.text[0]" :text2="languageData.text[1]" :text3="languageData.text[2]" :pointText1="languageData.pointText[0]" :pointText2="languageData.pointText[1]" />
      <languagePartTwo :text1="languageData.text[0]" :text2="languageData.text[3]" />
      <languagePartTwo :text1="languageData.text[0]" :text2="languageData.text[4]" :text3="languageData.text[5]" :pointText1="languageData.pointText[2]" :pointText2="languageData.pointText[3]" />
    </ul>
  </section>
</template>

<script>
import languagePart from "./LanguagePart.vue";
import languagePartTwo from "./LanguagePartTwo.vue";
import plateTitle from "./PlateTitle";
import data from "./data.json"
export default {
  components: { languagePart, languagePartTwo, plateTitle },
  data(){
    return {
      languageData: data.LanguageData,
      commonData: data.CommonData
      }
  }
};
</script>

<style>
</style>
