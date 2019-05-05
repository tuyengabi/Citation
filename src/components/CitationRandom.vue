<template>
  <div class="quotation">
    <img class="quotation__img" :src="quotes[index].adress">
    <p class="quotation__quote">{{ quotes[index].quote }}</p>
    <p class="quotation__author">{{ quotes[index].author }}</p>
     <v-btn class="quotation__btn" absolute="true" type="button" v-on:click="changeIndex" large>next</v-btn>
  </div>
</template>

<script>

import _ from 'lodash';

  export default {
    name: 'CitationRandom',
    data() {
      return {
        index: 0,
        quotes: [
          {
            adress: require('./../assets/img01.jpg'),
            author: "Albert Einstein",
            quote: "Learn from yesterday, live for today, hope for tomorrow. The important thing is not to stop questioning.",
          },

          {
            adress: require('./../assets/img02.jpg'),
            author: "Alan Watts",
            quote: "A person who never made a mistake never tried anything new.",
          },

          {
            adress: require('./../assets/img06.jpg'),
            author: "John Dewey",
            quote: "An ounce of experience is better than a ton of theory simply.",
          },

          {
            adress: require('./../assets/img1.jpg'),
            author: "Mark Twain",
            quote: "Life is short, break the rules.",
          },

          {
            adress: require('./../assets/img4.jpg'),
            author: "Paul F. Davis",
            quote: "Go where you’re celebrated, not where you’re tolerated.",
          },

          {
            adress: require('./../assets/img03.jpg'),
            author: "Samuel Goldwyn",
            quote: "The harder I work, the luckier I get.",
          },

          {
            adress: require('./../assets/img2.jpg'),
            author: "Ralph Waldo Emerson",
            quote: "Nothing great was ever achieved without enthusiasm.",
          },
        ]
    }
  },

    methods: {
      changeIndex : function() {
        this.index=_.random(0, 6)

      }

    }
}
</script>

<style>
.quotation {
  display: flex;
  position: relative;
  height: 100vh;
  width: 100vw;
  background-color: grey;
}
.quotation__img {
  width: 100%;
  object-fit: cover;
  object-position: center
}

.quotation__quote {
  color: orange;
  font-size: 3rem;
  margin-top: 10%;
  margin-left: 5%;
  margin-right: 5%;
  position: absolute;  
  text-shadow: 5px 5px 5px black;
}

.quotation__author {
  font-size: 2rem;
  font-weight: bold;
  font-style: italic;
  position: absolute;
  color: white;
  margin-top: 60vh;
  margin-left: 50%;
  text-shadow: 5px 5px 5px black;
}

.quotation__btn {
  border: 2px solid grey;
  color: grey;
  background-color: white;
  width: 7rem;
  font-size: 2rem;
  margin-top: 65vh !important;
  margin-left: 5% !important;
}
</style>
