<template>
    <div class="red">

        <p @click="saluto">Il mio primo componente</p>

    </div>
</template>

<script>
export default {
    name: 'FirstComponent',
    methods: {
        saluto() {
            console.log('il tuo primo componente ti saluta!')
        }
    }
}


</script>

<style scoped lang="scss">
.red {
    background-color: red;
}
</style>