<template>
  <section id="about" class="section">
    <div class=" has-text-centered">
      <div class="image avatar">
        <img src="../assets/img/nono.jpg">
      </div>
      <h2 class="title is-2">Nuno C. AMIAR</h2>
      <separator></separator>
      <div class="about-text block">
        <p>Born and raised in Portugal, I attended an unfinished course on physics in the best Portuguese University, IST. Now I’m permanently working in Algeria and well familiarized with the country's values.
        <br>
        <br>
        <p>My main interests are electronic vote and its implications in  political governance.</p>
          Specialized in decentralised software stack and identity management – Web 3.0.
      </div>
      
    </div>
  </section>
</template>

<script>
export default {
  name: 'about',
  data() {
    return {};
  },
  mounted() {
    sr.reveal('#about .block', 200);
  },
};
</script>

<style lang="scss">
  @import '~vars';

  .avatar {
    height: 200px;
    width: 200px;
    margin: 1rem auto;

    img {
      border-radius: 200px;
      border: 3px solid $secondary;
    }
  }

  .about-text {
    max-width: $tablet;
    margin: auto;
  }
</style>
