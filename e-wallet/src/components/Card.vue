<template>
<div>
    <p>Card.vue</p>
    <p>{{card.number}}</p>
</div>
</template>

<script>
export default {
    props: {
        card: Object,
    }
}
</script>

<style scoped>
</style>