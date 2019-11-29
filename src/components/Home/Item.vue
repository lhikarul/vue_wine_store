<template>
  <div class="items">
      <div class="item">
          <div class="img-wrapper">
              <img src="https://digitalcontent.api.tesco.com/v1/media/ghs/snapshotimagehandler_79244801.jpeg?h=540&w=540" alt="wine pic">
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
  </div>
</template>

<script>
export default {
    name: 'Item'
}
</script>

<style lang="scss" scoped>
@import "styles/placeholder";
    .items {
        margin: 0 auto;
        max-width: 315px;

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
                    color: #3F5D45;
                    font-size: 20px;
                }

                &-name {
                    flex: 0 0 183px;
                    border-right: 1px solid #EAF0ED;
                }

                &-price {
                    flex: 0 0 133.35px;
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
                color: #3F5D45;
                cursor: pointer;
                font-size: 24px;
                font-weight: 900;
                outline: none;
            }

            &-tag {
                box-sizing: border-box;
                padding: 10.5px;
                width: 37.8px;
                position: absolute;
                top: 0;
                left: 21px;
                background: #3F5D45;
                color: #fff;
            }

            &-icon {
                position: absolute;
                top: 0;
                right: 24px;
                font-size: 20px;
            }
        }
    }
</style>