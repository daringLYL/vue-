<template>
  <section class="experience">
    <div class="sec-title-wrapper">
      <h3 class="sec-title">
        <span class="sec-title-ch">项目与工作经验</span>
        <span class="sec-title-en">Experience</span>
      </h3>
    </div>
    <div class="timeline-wrapper">
      <ul class="sec-content timeline">
        <li class="timeline-item experience-internship">
          <h3 class="timeline-title">
            <span class="experience-place">
              Tekkers
              <span class="spaceFix"></span>极客团队
              <span class="spaceFix"></span>-
              <span class="spaceFix"></span>布里斯班
            </span>
            <time class="experience-time">
              2015.07
              <span class="spaceFix"></span>~
              <span class="spaceFix"></span>至今
            </time>
          </h3>
          <dl class="experience-description timeline-content">
            <expriencePart :title="exprienceData.title1" />
            <expriencePartTwo :pointType1="exprienceData.pointType1_One" :pointType2="exprienceData.pointType2_One" 
            :pointType3="exprienceData.pointType3_One" :pointType4="exprienceData.pointType4_One" :pointType5="exprienceData.pointType5_One" 
            :pointType6="exprienceData.pointType6_One" :type1="exprienceData.type1_One" :type2="exprienceData.type2_One" 
            :type3="exprienceData.type3_One" :type4="exprienceData.type4_One" :type5="exprienceData.type5_One" />
            <expriencePart :title="exprienceData.title2" />
            <expriencePartTwo :pointType1="exprienceData.pointType1_Two" :type1="exprienceData.type1_Two" :otherType1="exprienceData.otherType1_Two" 
            :otherType2="exprienceData.otherType2_Two" />
            <expriencePartTwo :pointType2="exprienceData.pointType2_Three" :pointType3="exprienceData.pointType3_Three" :type1="exprienceData.type1_Three"
            :type2="exprienceData.type2_Three" />
            <expriencePartTwo :pointType7="exprienceData.pointType7_Four" :type1="exprienceData.type1_Four" :otherType1="exprienceData.otherType1_Four" />
          </dl>
        </li>
        <li class="timeline-item experience-internship">
          <h3 class="timeline-title">
            <span class="experience-place">
              广联达兴安得力
              <span class="spaceFix"></span>-
              <span class="spaceFix"></span>上海
            </span>
            <time class="experience-time">
              2013.11
              <span class="spaceFix"></span>~
              <span class="spaceFix"></span>2014.02
            </time>
          </h3>
          <dl class="experience-description timeline-content">
            <expriencePart :title="exprienceData.title3" />
            <expriencePartTwo :pointType2="exprienceData.pointType2_Five" :pointType3="exprienceData.pointType3_Five" :pointType4="exprienceData.pointType4_Five" 
            :type1="exprienceData.type1_Five" :type2="exprienceData.type2_Five" :type3="exprienceData.type3_Five" />
            <expriencePartTwo :pointType2="exprienceData.pointType2_Six" :type1="exprienceData.type1_Six" :type2="exprienceData.type2_Six" />
          </dl>
        </li>
        <li class="timeline-item experience-project">
          <h3 class="timeline-title">
            <span class="experience-project-type">个人项目</span>
            <span class="experience-title-aside">
              <a
                href="https://github.com/n8659150/ProjectMinderWebApp"
                class="experience-project-link"
              >源代码</a>
              <a href="https://projectminder.firebaseapp.com" class="experience-project-link">Demo</a>
            </span>
          </h3>
          <dl class="experience-description timeline-content">
            <dt class="experience-project-name">
              Project
              <span class="spaceFix"></span>Minder
            </dt>
            <expriencePartTwo :pointType2="exprienceData.pointType2_Seven" :pointType3="exprienceData.pointType3_Seven" :type1="exprienceData.type1_Seven" />
            <expriencePartTwo :pointType1="exprienceData.pointType1_Eight" :pointType2="exprienceData.pointType2_Eight" 
            :pointType3="exprienceData.pointType3_Eight" :pointType4="exprienceData.pointType4_Eight" :pointType5="exprienceData.pointType5_Eight" 
            :pointType6="exprienceData.pointType6_Eight" :pointType7="exprienceData.pointType7_Eight" :type1="exprienceData.type1_Eight"
            :type2="exprienceData.type2_Eight" :type3="exprienceData.type3_Eight" :type4="exprienceData.type4_Eight" :type5="exprienceData.type5_Eight"
            :type6="exprienceData.type6_Eight" />
            <expriencePartTwo :pointType1="exprienceData.pointType1_Nine" :pointType2="exprienceData.pointType2_Nine" 
            :pointType3="exprienceData.pointType3_Nine" :pointType4="exprienceData.pointType4_Nine" :type1="exprienceData.type1_Nine" 
            :type2="exprienceData.type2_Nine" :type3="exprienceData.type3_Nine" />
            <expriencePartTwo :pointType1="exprienceData.pointType1_Ten" :pointType2="exprienceData.pointType2_Ten" :pointType3="exprienceData.pointType3_Ten" 
            :type1="exprienceData.type1_Ten" :type2="exprienceData.type2_Ten" :type3="exprienceData.type3_Ten" />
          </dl>
        </li>
        <li class="timeline-item experience-project">
          <h3 class="timeline-title">
            <span class="experience-project-type">个人项目</span>
            <span class="experience-title-aside">
              <a
                href="https://github.com/n8659150/ProjectMinderMobile"
                class="experience-project-link"
              >源代码</a>
            </span>
          </h3>
          <dl class="experience-description timeline-content">
            <dt class="experience-project-name">
              Project
              <span class="spaceFix"></span>Minder
              <span class="spaceFix"></span>Mobile
            </dt>
            <expriencePartTwo pointType7="配套手机应用" type1="Project" otherType1="Minder项目信息管理系统的"/>
            <expriencePartTwo pointType1="独自" pointType2="原有模块" pointType3="“用户会议管理”" pointType4="“学生地点定位”模块" 
            pointType5="手机端" pointType6="移植" pointType7="设计" pointType8="调试" pointType9="二次开发" type1="完成系统"
            type2="，新增" type3="，" type4="，" type5="界面的" type6="，" type7="，" type8="和" />
            <expriencePartTwo pointType1="独自" pointType2="20分钟英语" pointType3="12000字英语" 
            type1="完成" type2="项目汇报演讲及" type3="项目报告" />
            <expriencePartTwo pointType2="满分好评" pointType3="学校现有系统的新模块部署" type1="项目汇报演讲获导师" type2="并考虑作为" />
          </dl>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
import expriencePart from "./ExpriencePart.vue"
import expriencePartTwo from "./ExpriencePartTwo.vue"
import data from "./data.json"
export default {
   components: { expriencePart , expriencePartTwo },
   data() {
    return {
      exprienceData: data
    }
}};
</script>

<style>
</style>
