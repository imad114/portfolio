<template>
  <div class="personal">
    <h1>Personal Attributes..<span>.</span></h1>
    <ContainerBlock badge="badge1" text="Personal Projects">
      <h5>
        <a href="https://belance.netlify.app/" style="color: hsl(210, 100%, 66%);">Belance:</a> 
        This is a platform I developed where users can order a custom website tailored to their specific needs. 
        The service includes options for personalized design and team selection, making it a flexible solution for various website requirements.
      </h5>
      <h5>
        <a href="#" style="color: hsl(210, 100%, 66%);">Soul Swap:</a>
        This project is an online store dedicated to manga and anime characters. 
        It features an intuitive interface and user-friendly experience, designed to cater to fans and collectors alike.
      </h5>
    </ContainerBlock>
    <ContainerBlock badge="badge3" text="Languages">
      <div class="text">       
        Kablye: 
        <UiBadge styleBadge="badge" skill="high"/>
      </div>
      <div class="text">       
        English: 
        <UiBadge styleBadge="badge" skill="intermediate"/>
      </div>
      <div class="text">       
        French:  
        <UiBadge styleBadge="badge" skill="high"/>
      </div>
      <div class="text">       
        Arabe: 
        <UiBadge styleBadge="badge" skill="high"/>
      </div>
    </ContainerBlock>
  </div>
</template>

<script>
import ContainerBlock from './component/container.vue';
import UiBadge from '@/ui/badge.vue';

  export default {
    name: 'PersonalAttributes',
    components: {
      ContainerBlock,
      UiBadge
    }
  }
</script>

<style scoped>
  .personal {
    width: 40%;
    padding: 5rem 0;
    display: flex;
    align-items: start;
    justify-content: start;
    flex-direction: column;
    gap: 2rem;
    animation: toLeft 1.5s ease forwards;
  }

  span {
    animation: opacity 4s ease infinite;
  }

  h5, .text {
    font-weight: 400;
    color: var(--color-002);
    text-wrap: balance;
    word-spacing: 0.6em;
  }

  .text {
    width: 50%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-direction: row;
    font-size: clamp(12px, 2vw, 15px);
  }

  @media all and ( max-width: 1024px ) {
    .text {
      width: 100%;
    }
  }

  @media all and ( max-width: 768px ) {
    .personal {
      width: 100%;
      align-items: center;
      animation: toTop 1.5s ease forwards;
    }
  }
</style>