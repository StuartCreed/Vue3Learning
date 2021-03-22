<template>
    <section class="flex justify-between p-3 mr-32 ml-32">
        <SubHeader v-for="subHeader in subHeaders" :subHeader="subHeader" :activeTitle="activeTitle" @titleClick="titleClick"></SubHeader>
    </section>
</template>

<script>
import SubHeader from './SubHeader';
export default {
    components: {
        SubHeader
    },
    data() {
        return {
            subHeaders: {
                subHeader1: {
                    titles: ['Watch Live', 'Full Series', 'Shows', 'Categories' , 'News'],
                },
                subHeader2: {
                    titles: ['BritBox', 'Login']
                }
            },
            activeTitle: null // Dynamically set once mounted
        }
    },
    methods: {
        titleClick: function(title) {
            return this.activeTitle = title;
        }
    },
    mounted() {
        this.activeTitle = this.subHeaders.subHeader1.titles[0];
    }
}
</script>
K
