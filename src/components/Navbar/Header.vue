<template>
  <div class="Navbar-container__title elevation-24">
    <h1 class="Navbar-container__title-h1">Bracaval Elias</h1>
    <h2 class="Navbar-container__title-h2">Developer Full Stack Junior</h2>
    <a href="#">
      <v-icon class="Navbar-container__icon" @mouseover="hoverOver" @mouseleave="hoverLeave" :style="styles.icon">mdi-chevron-down</v-icon>
    </a>
  </div>
</template>

<script>

export default{
  name: 'Header',
  data() {
    return {
      styles : {
        icon : {
          fontSize : "6vw",
          top : "13vw",
          color : "#1d1d1d",
        }
      }
    };
  },
  methods: {
    hoverOver() {
      this.styles.icon.fontSize = "7vw";
      this.styles.icon.top = "12.7vw";
    }, 
    hoverLeave() {
      this.styles.icon.fontSize = "6vw";
      this.styles.icon.top = "13vw";
    }, 
  },
    
}

</script>

<style lang="scss" scoped>

.Navbar-container__title {
  display: flex;
  flex-direction: column;
  align-items: center;
  position: fixed;
  width: 35vw;
  height: 20vw;
  text-align: center;
  background-color: #d2d2d4;
  color: #1d1d1d;
  clip-path: polygon(50% 100%, 0 0, 100% 0);
  z-index: 1;

  .Navbar-container__title-h1 {
    position: relative;
    font-size: calc(1rem + 1.5vw);
    top: 4vw;
  }
  .Navbar-container__title-h2 {
    position: relative;
    font-size: calc(0.3rem + 1vw);
    margin-top: 1vw;
    top: 4vw;
  }

  .Navbar-container__icon {
    cursor: pointer;
    position: fixed;
    top: 13vw;
    left: 50%;
    transform: translate(-50%);
  }
}
</style>

