<template>
  <div class="work">
    <h1>Work Experience</h1>
    <ExperienceData
      style="animation: none;"
      :data="`2023 - 2024`"
      :position="`Freelance Full Stack Developer`"
      :text="`Worked on various client projects, building web applications and APIs using a range of technologies, including Vue,js,>dotnet, and MySQL.`"
    />
    <ExperienceData 
      style="animation: none;"
      :data="`Octobre 2024 - Present `"
      :position="`Full Stack Developer at Feco SPA`"
      :text="`Developed and maintained complex web applications using Vue js, DotNet, C#, and MySQl. Collaborated with cross-functional teams to deliver high-quality software solutions.`"
    />
    <router-link to="/about">
      <UiButton 
        text="View More" 
        :hoverColor="`hsl(275, 80%, 71%)`" 
        :hoverBgColor="`hsl(281, 38%, 16%)`" 
      />
    </router-link>
  </div>
</template>

<script>
import ExperienceData from './component/experience.vue';
import UiButton from '@/ui/btn.vue';

export default {
  name: 'WorkExperience',
  components: {
    ExperienceData,
    UiButton
  }
}
</script>

<style scoped>
.work {
  width: 80%;
  display: flex;
  align-items: start;
  justify-content: center;
  flex-direction: column;
  padding: 5rem 0;
  gap: 2rem;
}
</style>
