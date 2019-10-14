<template>
  <section class="language">
    <PlateTitle :title1="commonData.title.plateTitle[2]" :title2="commonData.title.plateTitle[3]" />
    <div class="sec-content">
      <dl class="language-certificates">
        <LanguagePart :language="languageData.language[0]" :level="languageData.level[0]" :width="languageData.width[0]" />
        <LanguagePart :language="languageData.language[1]" :level="languageData.level[1]" :width="languageData.width[1]" />
        <LanguagePart :language="languageData.language[2]" :level="languageData.level[2]" :width="languageData.width[2]" />
      </dl>
    </div>
    <ul class="language-description">
    <Information :text="commonData.text.textList[0]" :textClass="commonData.textClass[1]" />
    <Information :text="commonData.text.textList[1]" :textClass="commonData.textClass[1]" />
    <Information :text="commonData.text.textList[2]" :textClass="commonData.textClass[1]" />
    </ul>
  </section>
</template>

<script>
import LanguagePart from "./LanguagePart.vue";
import Information from "./Information.vue";
import PlateTitle from "./PlateTitle";
import data from "./data.json"
export default {
  components: { LanguagePart, Information, PlateTitle },
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
