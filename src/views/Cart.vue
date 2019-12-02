<template>
  <div class="cart-view">

        <div class="display-cart-orders-area">

            <div class="container">
                <div class="row">

                    <div class="column-md-8">

                            <h1 class="heading-title">你的購物車</h1>

                            <div class="cart-items-area">
                                <cart-item></cart-item>
                                <cart-item></cart-item>
                                <cart-item></cart-item>
                            </div>

                    </div>

                    <div class="column-md-4">
                            <h1 class="heading-title heading-bg">訂單摘要</h1>

                            <div class="order-items-area">
                                <order></order>
                            </div>

                            <h1 class="heading-title check">結帳</h1>
                    </div>

                </div>
            </div>

        </div>

  </div>
</template>

<script>
import CartItem from 'components/Cart/Item';
import Order from 'components/Cart/Order';
export default {
    name: 'Cart',
    components: {
        CartItem,
        Order
    }
}
</script>

<style lang="scss" scoped>
@import 'styles/const';

    // ----- grid ----- //
    .display-cart-orders-area {
        @media (min-width: 940px) {
            .container {
                max-width: 940px;
                margin: 0 auto;

                .row {
                    display: flex;

                    & > div:first-child {
                        margin-right: 20px;
                    }

                    .column-md-8 {
                        flex: 0 0 620px;
                        max-width: 620px;
                    }

                    .column-md-4 {
                        flex: 0 0 300px;
                        max-width: 300px;
                    }
                }
            }
        }
    }
    // ----- end of grid ----- //

    .cart-view {
        color: $primary-color;

        .heading-title {
            padding: 16px 0;
            background: $primary-light-color;
            color: $primary-color;
            text-align: center;

            &.check {
                margin-bottom: -30px;
                background-color: $gold;
            }

            &.heading-bg {
                @media (min-width: 940px) {
                    background-color: $primary-color;
                    color: $white;
                }
            }
        }

        .cart-items-area, .order-items-area {
            max-width: 315px;
            margin: 0 auto;

            @media (min-width: 940px) {
                max-width: 100%;
            }
        }

        .cart-items-area {
            padding: 30px 0;

            .cart-item-component {
                &:not(:first-child) {
                    padding-top: 30px;

                    @media (min-width: 940px) {
                        padding-top: 20px;    
                    }
                }
            }
        }

        .order-items-area {
            padding: 16px 0;

            @media (min-width: 940px) {
                padding: 0 18px;
                background: $primary-color;
                color: $white;
            }
        }
    }

</style>