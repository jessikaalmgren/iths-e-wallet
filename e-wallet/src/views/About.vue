<template>
  <div class="about">
    <h1>This is an about page</h1>
  <Top />
  <CardForm v-bind:value="card1" @add-card="handleEvent(data)" />
  <Card :card="card1" />
  

  </div>
</template>

<script>
import Top from "@/components/Top.vue"
import CardForm from "@/components/CardForm.vue"
import Card from "@/components/Card.vue"

export default {
  components: {
    Top,
    CardForm,
    Card,

  },

  data(){return{
    card1: {
      id: "432984728397",
      holder: "The name",
      vendor: "bitcoin",
      number: "XXXXYYYYZZZZFFFF",
      validMonth: "12",
      validDay: "5"
    },
    methods:{
        handleEvent(data){
          console.log(data)
        }
    },
    
  }}
}
</script>

<style scoped>

</style>