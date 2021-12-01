<template>
  <div id="app" v-cloak>
    <hero></hero>
    <about-us></about-us>
    <div class="skills columns is-multiline is-mobile" style="justify-content: center;">
        <div class="column is-half-mobile is-one-third-tablet is-one-quarter-desktop">
          <div class="skill">
              <about></about>
            </div>
        </div>
        <div class="column is-half-mobile is-one-third-tablet is-one-quarter-desktop">
          <div class="skill">
              <about2></about2>
            </div>
        </div>
      </div>
    
    <projects></projects>
    <skills></skills>
    <contact></contact>
    <copyright></copyright>
    <repo-modal></repo-modal>
  </div>
</template>

<script>
import Hero from './components/Hero';
import AboutUs from './components/AboutUs';
import About from './components/About';
import About2 from './components/About2';
import Projects from './components/Projects';
import Skills from './components/Skills';
import Contact from './components/Contact';
import Fork from './components/Fork';
import Copyright from './components/Copyright';
import RepoModal from './components/Projects/RepoModal';

export default {
  name: 'app',
  components: {
    Hero,
    About,
    About2,
    AboutUs,
    Projects,
    Skills,
    Fork,
    Contact,
    Copyright,
    RepoModal
  },
};
</script>

<style lang="scss">
#app {
  height: 100%;
  width: 100%;
  overflow: hidden;
}
</style>
