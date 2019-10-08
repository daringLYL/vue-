<template>
  <div class="timeline-wrapper">
    <ul class="sec-content timeline">
      <li class="timeline-item education-undergraduate">
        <h3 class="timeline-title">
          <time class="education-time">
            {{toTime}}
            <span class="spaceFix"></span>~
            <span class="spaceFix"></span>{{endTime}}
          </time>
        </h3>
        <dl class="education-description timeline-content">
          <dt class="education-name">昆士兰科技大学</dt>
          <dd class="education-major">
           {{subject}}
            <span class="spaceFix"></span>{{degree}}
          </dd>
          <dd class="education-honor">
            <strong>{{credit}}</strong>
            <span class="spaceFix"></span>/
            <span class="spaceFix"></span>7.0
            <span class="spaceFix"></span>GPA
          </dd>
          <dd class="education-hiscore">
            高分科目
            <span>
              <span class="spaceFix"></span>(6.0以上)
            </span>
          </dd>
          <dd style="margin-left:28px">{{outstandingSub}}</dd>
          <dd style="margin-left:28px">
            {{outstandingSub2}}
            <span class="spaceFix"></span>
            <span class="spaceFix"></span>等
          </dd>
        </dl>
      </li>
      
    </ul>
  </div>
</template>

<script>
export default {
  props:["toTime","endTime","subject","degree","credit","outstandingSub","outstandingSub2"]
};
</script>

<style>
</style>