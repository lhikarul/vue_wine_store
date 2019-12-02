<template>
  <div class="order-component">
        <ul  class="order-info">
            <li class="order-info-item"><span>小計</span><span>NT$ 2,700</span></li>
            <li class="order-info-item"><span>運費</span><span>NT$ 300</span></li>
            <li class="order-info-item total-order"><span>總計</span><span>NT$ 3,000</span></li>
        </ul>
  </div>
</template>

<script>
export default {
    name: 'Order'
}
</script>

<style lang="scss" scoped>
    @import "styles/const";

    .order-info {
        &-item {
            display: flex;
            justify-content: space-between;
        }

        &-item:nth-child(2) {
            margin-top: 8px;
            margin-bottom: 16px;
        }

        @media (min-width: 940px) {
            border-top: 1px solid $white;
            padding: 16px 0;
        }
    }

    .total-order {
        font-size: 20px;
        font-weight: 900;
    }
</style>