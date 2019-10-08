<template>
  <section class="language">
    <div class="sec-title-wrapper">
      <h3 class="sec-title">
        <span class="sec-title-ch">语言水平</span>
        <span class="sec-title-en">Language</span>
      </h3>
    </div>
    <div class="sec-content">
      <dl class="language-certificates">
        <languagePart :language="languageData.languageOne" :level="languageData.levelOne" :width="languageData.widthOne" />
        <languagePart :language="languageData.languageTwo" :level="languageData.levelTwo" :width="languageData.widthTwo" />
        <languagePart :language="languageData.languageThree" :level="languageData.levelThree" :width="languageData.widthThree" />
      </dl>
    </div>
    <ul class="language-description">
      <languagePartTwo :text1="languageData.text1_One" :text2="languageData.text2_One" :pointText1="languageData.pointText1_One" :pointText2="languageData.pointText2_One" />
      <languagePartTwo :text1="languageData.text1_Two" />
      <languagePartTwo :text1="languageData.text1_Three" :text2="languageData.text2_Three" :pointText1="languageData.pointText1_Three" :pointText2="languageData.pointText2_Three" />
    </ul>
  </section>
</template>

<script>
import languagePart from "./LanguagePart.vue";
import languagePartTwo from "./LanguagePartTwo.vue";
import data from "./data.json"
export default {
  components: { languagePart, languagePartTwo },
  data(){
    return {
      languageData:data
      }
  }
};
</script>

<style>
</style>
