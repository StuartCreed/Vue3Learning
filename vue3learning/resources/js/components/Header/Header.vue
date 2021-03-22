<template>
    <section class="flex justify-between p-3 mr-32 ml-32">
        <SubHeader v-for="subHeader in links" :links="subHeader"></SubHeader>
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
            links: {
                subHeader1: ['Watch Live', 'Full Series', 'Shows', 'Categories' , 'News'],
                subHeader2: ['BritBox', 'Login']
            }
        }
    }
}
</script>
K
