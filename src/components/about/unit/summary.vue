<template>
  <div class="summary">
    <h1>About Me..<span>.</span></h1>
    <ContainerBlock badge="badge1" text="summary">
      <h5>
        I am Imad Debiche, born in 1998.
        I work as a Full Stack Developer at  <a href="https://fecoit.com" style="color: hsl(210, 100%, 66%);">FECO SPA</a>. 
        I have one year of  experience working at FECO SPA . In addition to my professional role, I have also developed several personal projects.
       
      </h5>
    </ContainerBlock>
    <ContainerBlock badge="badge2" text="Additional Information">
      <h5>
        Dedicated to ongoing learning and professional growth, I thrive in dynamic environments and excel at tackling complex challenges.
      </h5>
    </ContainerBlock>
    <ContainerBlock badge="badge4" text="Education">
      <h5>
        I am a proud graduate of the University of Bejaia, where I specialized in computer science and advanced information systems. My education has provided me with a solid foundation in both fields, equipping me with the necessary skills to excel in the ever-evolving field of technology
      </h5>
    </ContainerBlock>
  </div>
</template>

<script>
import ContainerBlock from './component/container.vue'

  export default {
    name: 'SummaryPanel',
    components: {
      ContainerBlock
    }
  }
</script>

<style scoped>

  .summary {
    width: 40%;
    padding: 5rem 0;
    display: flex;
    align-items: start;
    justify-content: center;
    flex-direction: column;
    animation: toRight 1.5s ease forwards;
    gap: 2rem;
  }

  span {
    animation: opacity 4s ease infinite;
  }

  h5 {
    font-weight: 400;
    color: var(--color-002);
    text-wrap: balance;
    word-spacing: 0.6em;
  }

  @media all and ( max-width: 768px ) {
    .summary {
      width: 100%;
      align-items: center;
    }
  }

</style>