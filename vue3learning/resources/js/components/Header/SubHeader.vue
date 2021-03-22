<template>
    <section>
        <ul class="flex">
            <li v-for="title in titles" class="p-2">
                {{ title }}
            </li>
        </ul>
    </section>
</template>

<script>
    export default {
        props: ['titles']
    }
</script>
