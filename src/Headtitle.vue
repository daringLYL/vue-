<template>
 <h3 class="timeline-title">
            <span class="experience-place">
              {{experience1}}
              <span class="spaceFix"></span>{{experience2}}
              <span class="spaceFix"></span>{{shortLine1}}
              <span class="spaceFix"></span>{{experience3}}
              <span class="experience-title-aside">
              <a v-if="showLink1"
                :href="experienceProjectLink1"
                class="experience-project-link"
              >{{experienceProject1}}</a>
              <a v-if="showLink2" :href="experienceProjectLink2" class="experience-project-link">{{experienceProject2}}</a>
            </span>
            </span>
            <time class="experience-time">
              {{experienceToTime}}
              <span class="spaceFix"></span>{{shortLine2}}
              <span class="spaceFix"></span>{{experienceEndTime}}
            </time>
          </h3>
</template>

<script>
export default {
  props: ["experience1", "experience2", "experience3", "shortLine1", "shortLine2", "experienceToTime", "experienceEndTime",
  "experienceProjectLink1", "experienceProjectLink2", "experienceProject1", "experienceProject2", "showLink1", "showLink2"]
};
</script>

<style>
</style>

