<template>
  <nav class="Navbar-container__nav Navbar-container__nav-left elevation-12">
    <a class="Navbar-container__nav__link Navbar-container__nav-left__link Navbar-container__link-contact" href="#about">About</a>
    <a @click="animeSkills" class="Navbar-container__nav__link Navbar-container__nav-left__link Navbar-container__link-about" href="#skills">Skills</a>
  </nav>
</template>

<script>
export default{
  name: 'NavbarLeft',
  data() {
    return {
      toogleBool: true
    };
  },
  methods: {
    animeSkills() {
      if ( this.toogleBool) {
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

.Navbar-container__nav {
  display: flex;
  align-items: center;
  width: 35vw;
  height: 2.5vw;
  position: fixed;
  background-color: #bdbdbf;
  font-size: calc(1rem + 0.5vw);
  z-index: 1;
}

.Navbar-container__nav-left {
  padding: 0 5rem 0 1rem;
  left: 0;

  .Navbar-container__link-about {
    position: fixed;
    left: 24vw;
  }
  .Navbar-container__link-contact {
    position: fixed;
    left: 14vw;
  }
}

.Navbar-container__nav__link {
  position: relative;
  text-decoration: none;
  color: #1d1d1d;
}

</style>

