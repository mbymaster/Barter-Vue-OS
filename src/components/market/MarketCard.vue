<template>
 <div>
   <img :src=img64 alt="item image">
   <h1>{{title}}</h1>
   <h1 v-if="currencyBool">{{currencySymbol}}{{itemCurrencyValue.toFixed(2)}}</h1>
   <div v-if="barterBool">
     <div v-for="(item, index) in barterItems" :key="index">
       <span>{{item}} </span>
     </div>
   </div>
   <h1>Ships for {{currencySymbol}}{{shippingValue.toFixed(2)}}</h1>
   <h3>{{location}}</h3>
 </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'Blank',
  props: {
    id: Number,
    title: String,
    img64: String,
    currencyBool: Boolean,
    currencySymbol: String,
    itemCurrencyValue: Number,
    barterBool: Boolean,
    barterItems: Array,
    shippingBool: Boolean,
    shippingValue: Number,
    location: String
  }
})
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
