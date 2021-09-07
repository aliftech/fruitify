<template>
  <div class="about">
    <Fheader></Fheader>

    <main class="container">
      
      <div class="card">
        
        <div class="text-left">
          <p>Welcome to Fruitify, your number one source for all things Fruitify. We're dedicated to giving you the very best of Fruitify, with a focus on fruits data, and practice vue js.</p><br>

          <p>Founded in 2021 by Mr. Wahyu K. A., Fruitify has come a long way from its beginnings in Pacitan, East Java, Indonesia. When Mr. Wahyu first started out, his passion for eco-friendly cleaning products drove them to quit day job, do tons of research, etc. so that Fruitify can offer you the world's most advanced toothbrush. We now serve customers all over the world, and are thrilled that we're able to turn our passion into our own website.</p><br>

          <p>We hope you enjoy Our products as much as we enjoy offering them to you. If you have any questions or comments, please don't hesitate to contact us.</p><br>
        </div>

      </div>
    </main>

    <Footer></Footer>
  </div>
</template>

<script>

import Fheader from "../components/Fheader.vue";
import Footer from "../components/Footer.vue";

export default {
  name: 'About',
  components: {
    Fheader,
    Footer
  }
}
</script>

<style scoped>


</style>