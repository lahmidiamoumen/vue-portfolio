<template>
  <section id="about" class="section">
    <div class=" has-text-centered">
      <h2 class="title is-2">Who we are</h2>
      <separator></separator>
      <div class="about-text block">
        <p>
         <b>Numidia</b> was born with the vision of providing digital solutions to the problems of the everyday live of Algerian citizens. In particular our main area of research is the deployment of secure, cheap and massive consensus also known as the electronic vote. To achieve this goal we had to learn about blockchain technologies and distributed ledgers more broadly, from the level of the underlying hardware infrastructure to the deployment of the software with end-to-end cryptographic security.
        </p> <br> <p> This vision of bringing electronic vote to the masses also implied learning about correctly identifying individuals in different contexts while preserving their privacy and so we went on a learning journey that we’re still undergoing today.
        </p> <br> <p> Every human activity, whether political or purely economical can hugely benefit with the deployment of the right software that supports their operations.
   Using RFID technology or video vigilance cameras business owners can remain vigilant of their products from the comfort of their homes while managing their stock and human resources with customized management software.
	By having a small but background diverse team we can offer you our consulting services and are able to tailor our employees according to the necessities and size of the project at hands.

        </p><br>
        
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
