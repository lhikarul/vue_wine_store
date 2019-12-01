<template>
    <div class="banner-component">
        <div class="banner"></div>
    </div>
</template>

<script>
export default {
    name: 'Banner',
    props: {
        url: {
            type: String
        }
    },
    computed: {
        
    }
}
</script>

<style lang="scss" scoped>
    .banner {
        height: 277px;
        background: url(https://colorlib.com/preview/theme/wines/images/hero_1.jpg) no-repeat center center;
        background-size: cover;
    }
</style>