<template>
 <h3 class="timeline-title">
            <span class="experience-place">
              {{headtitle1}}
              <span class="spaceFix"></span>{{headtitle2}}
              <span class="spaceFix"></span>{{shortLine1}}
              <span class="spaceFix"></span>{{headtitle3}}
              <span class="experience-title-aside">
              <a v-if="showLink1"
                :href="projectLink1"
                class="experience-project-link"
              >{{project1}}</a>
              <a v-if="showLink2" :href="projectLink2" class="experience-project-link">{{project2}}</a>
            </span>
            </span>
            <time class="experience-time">
              {{toTime}}
              <span class="spaceFix"></span>{{shortLine2}}
              <span class="spaceFix"></span>{{endTime}}
            </time>
          </h3>
</template>

<script>
export default {
  props: ["headtitle1", "headtitle2", "headtitle3", "shortLine1", "shortLine2", "toTime", "endTime",
  "projectLink1", "projectLink2", "project1", "project2", "showLink1", "showLink2"]
};
</script>

<style>
</style>

