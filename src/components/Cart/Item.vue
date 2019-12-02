<template>
  <div class="cart-item-component">

        <div class="item">
            <div class="img-wrapper">
                <img src="https://images.unsplash.com/photo-1568623269068-c31912c211d4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=800&q=80" alt="cart item">
            </div>
            <div class="item-info">
                <div class="item-info-top">
                    <h3 class="item-info-title">Tesco Bordeaux</h3>
                    <p class="item-info-price">NT$ 450</p>
                </div>

                <div class="item-info-counts">
                    <a href="javascript:;">&laquo;</a>
                    <a href="javascript:;">1</a>
                    <a href="javascript:;">&raquo;</a>
                </div>
            </div>
        </div>

        <div class="extra-info">
            <span class="total-price">NT$ 900</span>
            <i class="fas fa-trash"></i>
        </div>

  </div>
</template>

<script>
export default {
    name: 'CartItem'
}
</script>

<style lang="scss" scoped>

@import "styles/const";

@media (max-width: 939px) {
    .fa-trash {
        display: none;
    }
}

.cart-item-component {
    @media (min-width: 940px) {
        display: flex;
        align-items: center;
        border-bottom: 1px solid $primary-light-color;
    }
}

.item {
    border-bottom: 1px solid $primary-light-color;
    padding-bottom: 8.5px;
    display: flex;

    .img-wrapper {
        flex: 0 0 50%;

        img {
            display: block;
            width: 100%;
            height: 106px;
        }
    }

    &-info {
        flex: 0 0 50%;
        box-sizing: border-box;
        padding-left: 16px;

        &-title {
            font-size: 20px;
        }

        &-counts {
            display: inline-block;
            margin-top: 18px;

            a {
                float: left;
                width: 45px;
                height: 45px;
                line-height: 45px;
                text-align: center;
                text-decoration: none;
                border: 1px solid #000;
                border-right: 0px;
                color: $primary-color;

                &:last-child {
                    border: 1px solid #000;
                }
            }
        }
    }

    @media (min-width: 940px) {
        border-bottom: none;
        padding-bottom: 20px;

        .img-wrapper {
            flex: 0 0 110px;
            max-width: 110px;

            img {
                width: 110px;
                height: 110px;
            }
        }

        &-info {
            padding-left: 39px;
            flex: 1;
            display: flex;
            align-items: center;

            &-counts {
                margin-top: 0;
                padding-left: 39px;
            }
        }
    }
}

.extra-info{
    border-bottom: 1px solid $primary-light-color;
    padding: 8.5px 0;
    font-size: 20px;
    text-align: right;

    @media (min-width: 940px) {
        border-bottom: none;
        padding-top: 0;
        padding-bottom: 20px;

        .total-price {
            padding: 0 25px;
        }
    }
}
    
</style>