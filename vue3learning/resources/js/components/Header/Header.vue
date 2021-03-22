<template>
    <section class="flex justify-between p-3 mr-32 ml-32">
        <SubHeader :links="subHeader1Links"></SubHeader>
        <SubHeader :links="subHeader2Links"></SubHeader>
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
            subHeader1Links: ['Watch Live', 'Full Series', 'Shows', 'Categories' , 'News'],
            subHeader2Links: ['BritBox', 'Login']
        }
    }
}
</script>
