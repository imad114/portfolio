<template>
  <footer>
    <div class="left-footer">
      <h3><font-awesome-icon icon="code" /></h3>
      <h3>Debiche Imad</h3>
    </div>
    <div class="right-footer">
      <a href="https://github.com/Takemyeye">
        <h3><font-awesome-icon icon="fa-brands fa-github" /></h3>
      </a>
      <a href="https://t.me/+_A-d1T6L8a02NzU0">
        <h3><font-awesome-icon icon="fa-brands fa-telegram" /></h3>
      </a>
      <a href="https://www.instagram.com/takemyeyegit/">
        <h3><font-awesome-icon icon="fab fa-instagram" /></h3>
      </a>
      <a href="">
        <h3><font-awesome-icon icon="fa-brands fa-linkedin" /></h3>
      </a>
    </div>
  </footer>
</template>

<script>
  export default {
    name: 'FooterPanel'
  }
</script>

<style scoped>
  footer {
    width: 100%;
    background-color: hsl(240, 2%, 9%);
    display: flex;
    align-items: center;
    justify-content: space-around;
    padding: 1.5rem 0;
    gap: 30%;
  }
  .left-footer, .right-footer {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: row;
    gap: 1rem;
  }

  @media all and ( max-width: 768px ) {
    footer {
      gap: 5%;
    }
  }

</style>