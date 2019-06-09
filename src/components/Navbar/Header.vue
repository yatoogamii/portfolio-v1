<template>
  <div class="Navbar-container__title">
    <h1 class="Navbar-container__title-h1">Bracaval Elias</h1>
    <h2 class="Navbar-container__title-h2">Developer Full Stack Junior</h2>
    <a @click="fullpageDown" :href="anchor.link">
      <v-icon class="Navbar-container__icon" @mouseover="hoverOver" @mouseleave="hoverLeave" :style="styles.icon">mdi-chevron-down</v-icon>
    </a>
  </div>
</template>

<script>

export default{
  name: 'Header',
  data() {
    return {
      anchor: {
        link : ""
      },
      count: 0,
      styles : {
        icon : {
          fontSize : "6vw",
          top : "13vw",
          color : "#1d1d1d",
        }
      },
      toogleBool: true
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
    setAnchorLink() {
      const aboutPos = document.getElementsByClassName('about')[0].getBoundingClientRect().y;
      const skillsPos = document.getElementsByClassName('skills')[0].getBoundingClientRect().y;
      const projectPos = document.getElementsByClassName('project')[0].getBoundingClientRect().y;
      const projectNextPos = document.getElementsByClassName('project-next')[0].getBoundingClientRect().y;
      const contactPos = document.getElementsByClassName('contact')[0].getBoundingClientRect().y;

      if (aboutPos > 0) {
        this.anchor.link = "#about";
      } else if(skillsPos > 0){
        this.anchor.link = "#skills";
      } else if(projectPos > 0) {
        this.anchor.link = "#project";
      } else if(projectNextPos > 0) {
        this.anchor.link = "#project-next";
      } else if(contactPos > 0) {
        this.anchor.link = "#contact";
      } else {
        this.anchor.link = "#about";
      }

    },
    fullpageDown() {
      const aboutPos = document.getElementsByClassName('about')[0].getBoundingClientRect().y;
      const skillsPos = document.getElementsByClassName('skills')[0].getBoundingClientRect().y;
      const projectPos = document.getElementsByClassName('project')[0].getBoundingClientRect().y;
      const projectNextPos = document.getElementsByClassName('project-next')[0].getBoundingClientRect().y;
      const contactPos = document.getElementsByClassName('contact')[0].getBoundingClientRect().y;

      const allPos = ["#about", "#skills", "#project", "#project-next", "#contact"];
      this.anchor.link = allPos[this.count > allPos.length - 1 ? this.count = 0 : this.count];
      this.count++;
      this.animeSkills();
    },
    fullpageUp() {
      const aboutPos = document.getElementsByClassName('about')[0].getBoundingClientRect().y;
      const skillsPos = document.getElementsByClassName('skills')[0].getBoundingClientRect().y;
      const projectPos = document.getElementsByClassName('project')[0].getBoundingClientRect().y;
      const projectNextPos = document.getElementsByClassName('project-next')[0].getBoundingClientRect().y;
      const contactPos = document.getElementsByClassName('contact')[0].getBoundingClientRect().y;

      const allPos = [aboutPos, skillPos, projectPos, projectNextPos, contactPos];
      this.anchor.link = allPos[this.count--];
      this.animeSkills();
    },
    animeSkills() {
      if ( this.toogleBool && this.anchor.link == '#skills') {
        this.toogleBool = false;
        setTimeout(() => { 
          const github = document.getElementsByClassName('github')[0].ldBar;
          const css = document.getElementsByClassName('css')[0].ldBar;
          const linux = document.getElementsByClassName('linux')[0].ldBar;
          const vim = document.getElementsByClassName('vim')[0].ldBar;
          const react = document.getElementsByClassName('react')[0].ldBar;
          const vuejs = document.getElementsByClassName('vuejs')[0].ldBar;
          const postgresql = document.getElementsByClassName('postgresql')[0].ldBar;
          const js = document.getElementsByClassName('js')[0].ldBar;
          github.set(0)
          github.set(70)
          css.set(0)
          css.set(80)
          linux.set(0)
          linux.set(70)
          vim.set(0)
          vim.set(80)
          react.set(0)
          react.set(50)
          vuejs.set(0)
          vuejs.set(60)
          js.set(0)
          js.set(70)
          postgresql.set(0)
          postgresql.set(60)
        }, 500);
      }
    }
  }
}

</script>

<style lang="scss" scoped>

.Navbar-container__title {
  display: flex;
  flex-direction: column;
  align-items: center;
  position: fixed;
  left: 50vw;
  transform: translate(-50%);
  width: 35vw;
  height: 20vw;
  background-color: #d2d2d4;
  color: #1d1d1d;
  clip-path: polygon(50% 100%, 0 0, 100% 0);
  z-index: 2;

  .Navbar-container__title-h1 {
    position: relative;
    font-size: calc(1rem + 1.5vw);
    top: 4vw;
  }
  .Navbar-container__title-h2 {
    position: relative;
    font-size: calc(0.2rem + 1vw);
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

