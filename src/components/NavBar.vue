<template>
  <header class="nav">
    <div class="container">
      <div class="nav-left">
        <a class="nav-item "
          rel="noopener"
          href="#">
          <img src="../assets/img/sr-logo.png" alt="skill" />
        </a>
      </div>
      <span class="nav-toggle"
        :class="{'is-active' : isExpanded }"
        @click="isExpanded = !isExpanded">
        <span></span>
        <span></span>
        <span></span>
      </span>
      <div class="nav-right nav-menu"
        :class="{ 'is-active': isExpanded }">
        <a v-for="(item, index) in menuItems"
          class="nav-item"
          href="#"
          :key="index"
          @click.prevent="goTo(item)">
          {{ item.title }}
        </a>
      </div>
    </div>
  </header>
</template>

<script>



export default {
  name: 'navbar',
  data() {
    return {
      logo: 'NUMIDIA',
      isExpanded: false,
      menuItems: [
        {
          title: 'About',
          el: '#about',
        }, 
        {
          title: 'e-gov',
          el: '#projects',
        }, {
          title: 'Tchnologies',
          el: '#skills',
        }, {
          title: 'Contact',
          el: '#contact',
        },
      ],
    };
  },
  methods: {
    goTo(item) {
      this.isExpanded = false;
      if (item.url) {
        window.location.assign(item.url);
      } else {
        this.$scrollTo(item.el);
      }
    },
  },
};
</script>

<style lang="scss">
  .logo-text {
    font-family: Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    font-size: 20px;
    font-style: blod;
    
  }
</style>
