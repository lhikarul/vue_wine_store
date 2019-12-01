<template>
  <div class="items-container">
      <item></item>
      <item></item>
      <item></item>
  </div>
</template>

<script>
import Item from 'base/Item';

export default {
    name: 'Items',
    components: {
        Item
    }
}
</script>

<style lang="scss" scoped>

.items-container {
    margin: 0 auto;
    max-width: 315px;

    .item {
        margin-top: 30px;
    }

    @media (min-width: 940px) {
        display: flex;
        flex-wrap: wrap;
        max-width: 100%;

        .item {
            flex: 0 0 50%;
            max-width: 50%;
            box-sizing: border-box;
            margin-top: 0;
            margin-bottom: 20px;
            padding-left: 20px;
        }
    }
}

</style>