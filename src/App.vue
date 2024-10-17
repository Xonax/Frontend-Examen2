<template>
  <nav class="d-none align-items-center  justify-content-center d-sm-flex">
    <router-link class="p-2" to="/">Homepagina</router-link>
    <router-link class="p-2" to="/Algemene-informatie">Algemene informatie</router-link>
    <router-link class="p-2" to="/Overzichtspagina">Overzichtspagina</router-link>
    <router-link class="p-2" to="/Nieuws">Nieuws</router-link>
    <router-link class="p-2" to="/Contactformulier">Contactformulier</router-link>
  </nav>
  <responsive-nav class="d-flex d-sm-none align-items-center justify-content-between px-3">
    <img class="logo" src="../src/assets/logo.png" alt="Cocktailbar Melontime">
    <div class="hamburger d-flex" @click="toggleNav('open')">
      <span></span>
      <span></span>
      <span></span>
    </div>
  </responsive-nav>

  <mobile-nav class="w-100 h-100 d-sm-none d-flex "
    :class="{ 'nav-open': isNavOpen }">

    <div class="d-flex flex-column">
      <router-link class="p-2" to="/">Homepagina</router-link>
      <router-link class="p-2" to="/Algemene-informatie">Algemene informatie</router-link>
      <router-link class="p-2" to="/Overzichtspagina">Overzichtspagina</router-link>
      <router-link class="p-2" to="/Nieuws">Nieuws</router-link>
    <router-link class="p-2" to="/Contactformulier">Contactformulier</router-link>

    </div>
    <div class="close ms-auto me-2" @click="toggleNav('close')">
      <svg xmlns="http://www.w3.org/2000/svg" x="0px" y="0px" width="25" height="25" viewBox="0 0 30 30">
          <path d="M 7 4 C 6.744125 4 6.4879687 4.0974687 6.2929688 4.2929688 L 4.2929688 6.2929688 C 3.9019687 6.6839688 3.9019687 7.3170313 4.2929688 7.7070312 L 11.585938 15 L 4.2929688 22.292969 C 3.9019687 22.683969 3.9019687 23.317031 4.2929688 23.707031 L 6.2929688 25.707031 C 6.6839688 26.098031 7.3170313 26.098031 7.7070312 25.707031 L 15 18.414062 L 22.292969 25.707031 C 22.682969 26.098031 23.317031 26.098031 23.707031 25.707031 L 25.707031 23.707031 C 26.098031 23.316031 26.098031 22.682969 25.707031 22.292969 L 18.414062 15 L 25.707031 7.7070312 C 26.098031 7.3170312 26.098031 6.6829688 25.707031 6.2929688 L 23.707031 4.2929688 C 23.316031 3.9019687 22.682969 3.9019687 22.292969 4.2929688 L 15 11.585938 L 7.7070312 4.2929688 C 7.5115312 4.0974687 7.255875 4 7 4 z"></path>
      </svg>
    </div>
  </mobile-nav>
  

  <router-view/>
</template>

<style>
/*

  main
  #9B8AC8
  #C4BBF0
  #665490

*/

svg path {
  fill: #fff;
}

.nav-open {
  top: 0% !important;
}

mobile-nav {
  position: fixed;
  top: -200%;
  z-index: 999;
  background-color: #665490;
}
mobile-nav a {
  color: #fff;
}

.hamburger span {
  background-color: #fff;
  width: 25px;
  height: 4px;
  border-radius: 40rem;
}

.hamburger span + span:not(span + span + span) {
  margin-block: 4px;
}

.hamburger {
  flex-direction: column;
}

.logo {
  width: 75px;
  aspect-ratio: 1;
}
section {
  padding-block: 10vh;
}

nav {
  min-height: 15vh;
}

nav a {
  background-color: white;
  color: black;
  margin-inline: 1rem;
  text-decoration: none;
  border-radius: 50rem;
  min-width: 6rem;
  text-align: center
}

nav a:hover {
  transition: all .3s;
  background-color: rgb(212, 212, 212);
}

body {
  margin: 0;
  background-color: #C4BBF0 !important;
}

p,
h1,
h2,
h3,
h4,
h5,
h6 {
  color: #fff !important;
}

</style>

<script>
export default {
  data() {
    return {
      isNavOpen: false,
    };
  },
  methods: {
    toggleNav(type) {
      if (type === "close") {
        this.isNavOpen = false;
      } else if (type === "open") {
        this.isNavOpen = true;
      }
    }
  }
};
</script>
