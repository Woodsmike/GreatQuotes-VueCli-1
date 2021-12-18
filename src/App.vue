<template>  
    <div class="container">
      <new-quote @quoteAdded="newQuote"></new-quote>
      <app-quote-grid :quotes="quotes"></app-quote-grid>
      </div> 
</template>

<script>
  import QuoteGrid from './components/QuoteGrid.vue';
  import NewQuote from './components/NewQuote.vue';

  export default {
    data: function () {
      return {
        quotes: [
          'Just something to hold text',
          'Another quote of nothing'
        ],
        maxQuotes: 10
      }
    },
    components : {
      appQuoteGrid : QuoteGrid,
      newQuote: NewQuote
    },
    methods : {
      newQuote (quote){
        this.quotes.push(quote)
      }
    }
  }
</script>

<style>

</style>
