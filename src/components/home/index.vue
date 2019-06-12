<template>
  <div>
    <app-header/>
    <app-about/>
    <app-skills-education/>
    <app-portfolio/>
    <app-experience/>
    <app-contact/>
    <app-footer/>
  </div>
</template>

<script>
  import appHeader from './Header.vue';
  import appAbout from './About.vue';
  import appSkillsEducation from './SkillsEducation.vue';
  import appExperience from './Experience.vue';
  import appPortfolio from './Portfolio.vue';
  import appContact from './Contact.vue';
  import appFooter from '../core/Footer1.vue';

  export default {
    components: {
      appHeader,
      appAbout,
      appSkillsEducation,
      appExperience,
      appPortfolio,
      appContact,
      appFooter
    }
  }
</script>

