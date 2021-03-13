<template>
    <ul class="testing bg-green-500 flex justify-evenly align-middle">
        <li v-for="item in items">{{ item }}</li>
    </ul>
</template>

<script>
export default {
    data() {
        return {
            items: {
                first: 'banana',
                second: 'apple',
                third: 'orange'
            }
        }
    }
}

</script>

<style scoped>
    .testing {
        color: var(--theme-color-two)
    }
</style>
