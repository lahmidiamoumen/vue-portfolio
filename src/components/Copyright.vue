<template>
  <footer class="footer">
    <div class="container">
      <div class="content has-text-centered">
        <p>
          © 2021 Numidia
        </p>
        <p>
          <a class="icon"
            v-for="(item,index) in social"
            :href="item.link"
            :key="index"
            target="_blank"
            rel="noopener">
            <b-icon :icon="item.icon"></b-icon>
          </a>
        </p>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'copyright',
  data() {
    return {
      social: [
        {
          icon: 'linkedin',
          link: '#',
        },
        {
          icon: 'twitter',
          link: '#',
        },
        {
          icon: 'github',
          link: '#',
        },
        {
          icon: 'gitlab',
          link: '#',
        },
        {
          icon: 'codepen',
          link: '#',
        },
      ],
    };
  },
};
</script>

