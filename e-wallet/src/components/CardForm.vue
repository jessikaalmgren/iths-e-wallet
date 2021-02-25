<template>
<div>
    <h1>cardform.vue</h1>
    <p>You have new</p>
    <form>
        <input v-model="value.number" placeholder="input" >
        <p>Message is: {{value}}</p>
        <button @click="handleEvent">Skicka</button>
        <!--<p>{{value}}</p>-->
        
    </form>
    
</div>
</template>

<script>
export default {
    props: {
        value: Object,

    },
    data(){return{
        hello: "",
    }},
    methods: {
        handleEvent(){
            console.log("clicked")
            this.$emit('addCard', this.props.value )
        }
    }
}
</script>

<style scoped>
</style>