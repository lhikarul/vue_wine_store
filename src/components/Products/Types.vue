<template>
  <div>
      <ul class="types-wrapper">
          <li class="item-type">類別</li>
          <li class="item-type">所有藏酒(48)</li>
          <li class="item-type">本日精選(10)</li>
          <li class="item-type">人氣推薦(26)</li>
          <li class="item-type">新品上市(12)</li>
      </ul>
  </div>
</template>

<script>
export default {
    name: 'Types'
}
</script>

<style lang="scss" scoped>
@import "styles/const";

    .types-wrapper {
        text-align: center;
        .item-type {
            padding: 15px 0;
            height: 35px;
            /* line-height: 65px; */
            color: $primary-color;
            font-size: 24px;
        }

        li:first-child {
            background: $primary-color;
            color: $white;
        }

    }
</style>