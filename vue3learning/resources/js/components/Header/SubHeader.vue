<template>
    <section>
        <ul class="flex">
            <li v-for="title in subHeader.titles" class="p-2" :class="{active: isActive(title)}" @click="clicked(title)">
                {{ title }}
            </li>
        </ul>
    </section>
</template>

<script>
    export default {
        props: ['subHeader', 'activeTitle'],
        methods: {
            isActive: function(title) {
                return title === this.activeTitle
            },
            clicked: function(title) {
                return this.$emit('titleClick', title)
            }
        }
    }
</script>

<style scoped>
    .active {
        color: var(--active)
    }
</style>
