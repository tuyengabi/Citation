<template>
  <div class="page">
    <img class="img" src="adress">
    <p class="qte">{{ quote }}</p>
    <p class="atr">{{ author }}</p>
  </div>
</template>

<script>
  export default {
    name: 'CitationRandom',
    data() {
      return {
        quotes: [
          {
            adress: "../assets/img01.jpg",
            author: "Albert Einstein",
            quote: "Learn from yesterday, live for today, hope for tomorrow. The important thing is not to stop questioning.",
          },

          {
            adress: "../assets/img02.jpg",
            author: "Albert Einstein",
            quote: "Learn from yesterday, live for today, hope for tomorrow. The important thing is not to stop questioning.",
          },

          {
            adress: "../assets/img03.jpg",
            author: "Albert Einstein",
            quote: "Learn from yesterday, live for today, hope for tomorrow. The important thing is not to stop questioning.",
          },

          {
            adress: "../assets/img04.jpg",
            author: "Albert Einstein",
            quote: "Learn from yesterday, live for today, hope for tomorrow. The important thing is not to stop questioning.",
          },

          {
            adress: "../assets/img05.jpg",
            author: "Albert Einstein",
            quote: "Learn from yesterday, live for today, hope for tomorrow. The important thing is not to stop questioning.",
          },

          {
            adress: "../assets/img06.jpg",
            author: "Albert Einstein",
            quote: "Learn from yesterday, live for today, hope for tomorrow. The important thing is not to stop questioning.",
          },

          {
            adress: "../assets/img1.jpg",
            author: "Albert Einstein",
            quote: "Learn from yesterday, live for today, hope for tomorrow. The important thing is not to stop questioning.",
          },
        ]
    }
  }
</script>

<style>

</style>
