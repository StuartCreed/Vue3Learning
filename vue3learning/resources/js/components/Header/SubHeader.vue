<template>
    <section>
        <ul class="flex">
            <li v-for="link in links" class="p-2">
                {{ link }}
            </li>
        </ul>
    </section>
</template>

<script>
    export default {
        props: ['links']
    }
</script>
