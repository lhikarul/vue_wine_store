<template>
    <header class="header">
        <div class="header-left">
            <i class="fas fa-bars icon"></i>
        </div>

        <div class="header-middle">
            <img class="logo-img" src="https://colorlib.com/preview/theme/wines/images/logo.png" alt="logo">
        </div>

        <div class="header-right">
            <i class="fas fa-shopping-cart icon"></i>
        </div>

    </header>
</template>

<script>
export default {
    name: 'VHeader'
}
</script>

<style lang="scss" scoped>
    .header {
        padding: 30px;
        display: flex;
        align-items: center;
        justify-content: space-between;
        
        .logo-img {
            width: 140px;
        }

        .icon {
            font-size: 24px;
        }
    }
</style>