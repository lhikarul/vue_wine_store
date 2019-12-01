<template>
      <div class="item">
          <div class="img-wrapper">
              <img src="https://images.unsplash.com/photo-1568623269068-c31912c211d4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=800&q=80" alt="wine pic">
          </div>
          <div class="item-info">
              <h3 class="item-info-name">Tesco Bordeaux</h3>
              <div class="item-info-price">NT$ 450</div>
          </div>
          <div class="item-btn">
              <button>加入購物車</button>
          </div>

          <div class="item-tag">
              <span>本日精選</span>
          </div>

          <div class="item-icon"><i class="far fa-heart"></i></div>
      </div>
</template>

<script>
export default {
    name: 'Item'
}
</script>

<style lang="scss" scoped>
@import "styles/const";
@import "styles/placeholder";

    .item {
        position: relative;
        
        .img-wrapper img {
            width: 100%;
        }

        &-info {
            border: 1px solid #EAF0ED;
            height: 56px;
            display: flex;
            justify-content: space-between;

            &-name,&-price {
                @extend %flex-center;
                color: $primary-color;
                font-size: 20px;
            }

            &-name {
                flex: 0 0 58%;
                border-right: 1px solid #EAF0ED;
            }

            &-price {
                flex: 0 0 42%;
                font-weight: 900;
            }

        }

        &-btn button {
            border: 1px solid #EAF0ED;
            border: none;
            display: block;
            width: 100%;
            height: 100%;
            height: 65px;
            background: #EAF0ED;
            color: $primary-color;
            cursor: pointer;
            font-size: 24px;
            font-weight: 900;
            outline: none;
        }

        &-tag {
            box-sizing: border-box;
            margin-left: 20px;
            padding: 10.5px;
            width: 37.8px;
            position: absolute;
            top: 0;
            background: $primary-color;
            color: $white;
        }

        &-icon {
            position: absolute;
            top: 0;
            right: 24px;
            font-size: 20px;
        }
    }
    
</style>