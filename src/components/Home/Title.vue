<template>
  <div>
        <h1 class="heading-title"><span class="position">{{title}}-----</span>
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
    padding-bottom: 30px;
    color: #3F5D45;
    font-size: 24px;
    letter-spacing: 2px;
    text-align: center;
}

@media (min-width: 940px) {
    .heading-title {
        padding: 0;
        font-size: 32px;
        text-align: left;
    }

    .position {
        margin-top: -20px;
    }
}

</style>