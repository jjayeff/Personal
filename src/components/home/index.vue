<template>
  <div>
    <app-header/>
    <app-about/>
    <app-skills-education/>
    <app-portfolio/>
    <app-experience/>
  </div>
</template>

<script>
  import appHeader from './Header.vue';
  import appAbout from './About.vue';
  import appSkillsEducation from './SkillsEducation.vue';
  import appExperience from './Experience.vue';
  import appPortfolio from './Portfolio.vue';

  export default {
    components: {
      appHeader,
      appAbout,
      appSkillsEducation,
      appExperience,
      appPortfolio
    }
  }
</script>

