<template>
  <section id="about" class="section">
    <div class=" has-text-centered">
      <div class="image avatar">
        <img src="https://lahmidiamoumen.github.io/img/moune_edit.jpg">
      </div>
      <h2 class="title is-2">Lahmidi A.mounmen</h2>
      <separator></separator>
      <div class="about-text block">
        <p>Master degree on Computer Sciences University of Boumerdes. I'm dedicated to promoting the discipline of delivering quality software.</p>
        <br>
        <br>
        <p>My domain of interests are blockchain and machine learning technologies and there applications in e-governance and healthcare.</p>
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
