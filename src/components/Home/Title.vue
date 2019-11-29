<template>
  <div>
        <h1 class="heading-title">{{title}}-----
            <br>
            {{subTitle}}
        </h1>
  </div>
</template>

<script>
export default {
    name: 'HeadingTitle',
    props: {
        title: {
            type: String,
            default: '為什麼'
        },
        subTitle: {
            type: String,
            default: ''
        }
    }
}
</script>

<style lang="scss" scoped>

.heading-title {
    margin: 30px 0;
    color: #3F5D45;
    font-size: 24px;
    letter-spacing: 2px;
    text-align: center;
}

</style>