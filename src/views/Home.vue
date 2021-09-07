<template>
  <div class="home">

    <Header v-on:random-fruits="changeFruits"></Header>

    <main>
      
      <article v-if="!fruit">
        <Fruits :fruits="item" v-for="(item, index) in fruits" :index="index" :key="item.id"></Fruits>
      </article>
      <article v-else>
        <Fruits :fruits="fruit" :index="0"></Fruits>
      </article>
    </main>

    <Footer></Footer>

  </div>
</template>

<script>

import Header from "../components/Header.vue"
import Footer from "../components/Footer.vue"
import Fruits from "../components/Fruits.vue";

export default {
  name: 'Home',
  components: {
    Header,
    Footer,
    Fruits
  },
  data() {
    return {
      fruits: [
        {
          id: 1,
          name: 'Apple',
          taste: 'Sweet',
          image: 'apple.jpg'
        },
        {
          id: 2,
          name: 'Banana',
          taste: 'Sweet',
          image: 'banana.jpg'
        },
        {
          id: 3,
          name: 'Cerry',
          taste: 'Sweet/Sour',
          image: 'cerry.jpg'
        },
        {
          id: 4,
          name: 'Durian',
          taste: 'Sweet',
          image: 'durian.jpg'
        },
        {
          id: 5,
          name: 'Grape',
          taste: 'Sweet/Sour',
          image: 'grape.jpg'
        },
        {
          id: 6,
          name: 'Lemon',
          taste: 'Sour',
          image: 'lemon.jpg'
        },
        {
          id: 7,
          name: 'Leccy',
          taste: 'Sweet/Sour',
          image: 'leccy.jpg'
        },
        {
          id: 8,
          name: 'Mango',
          taste: 'Sweet/Sour',
          image: 'mango.jpg'
        },
        {
          id: 9,
          name: 'Orange',
          taste: 'Sweet/Sour',
          image: 'orange.jpg'
        },
        {
          id: 10,
          name: 'Pineapple',
          taste: 'Sour',
          image: 'pineapple.jpg'
        },
        {
          id: 11,
          name: 'Papaya',
          taste: 'Sweet',
          image: 'papaya.jpg'
        }
      ],
      fruit: '',
      search: ''
    }
  },
  methods: {
    changeFruits() {
      this.fruit = this.randomFruits()
    },
    randomFruits() {
      return this.fruits[Math.floor(Math.random() * this.fruits.length)]
    }
  }
}
</script>

<style>
  article {
    display:flex;
    flex-wrap: wrap;
    justify-content: center;
  }

  article img {
    width: 200px;
    height: 200px;
    padding: 20px 20px;
  }

  article li {
    list-style-type: none;
    text-align: center;
  }

  p {
    color:slategrey;
  }

  h3 {
    color:slategrey;
    font-weight: bold;
  }

  .card {
    margin: 10px 10px;
    padding: 20px 20px;
  }

</style>