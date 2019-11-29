<template>
  <div>
      <ul class="list-wrapper">
          <li  class="list-item list-item-1">
              <router-link to="/" class="list-item-text">本日精選</router-link>
          </li>
          <li  class="list-item list-item-2">
              <router-link to="/" class="list-item-text">人氣推薦</router-link>
          </li>
          <li  class="list-item list-item-3">
              <router-link to="/" class="list-item-text">新品上市</router-link>
          </li>
      </ul>
  </div>
</template>

<script>
export default {
    name: 'List'
}
</script>

<style lang="scss" scoped>
    .list-wrapper {
        display: flex;
        align-items: center;
        justify-content: space-between;
        
        .list-item {

            flex: 1;
            height: 180px;
            position: relative;

            &:after {
                content: '';
                display: block;
                position: absolute;
                top: 0;
                right: 0;
                bottom: 0;
                left: 0;
                background: #3F5D45;
                opacity: .9;
            }

            &-text {
                width: 20px;
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%,-50%);
                z-index: 1;
                color: #fff;
                font-size: 20px;
                text-decoration: none;
            }

            &-1 {
                    background: url(https://colorlib.com/preview/theme/wines/images/wine_1.png) no-repeat center center;

                    &:after {
                        background: #FFE180;
                    }

                    .list-item-text {
                        color: #3F5D45;
                        font-weight: bold;
                    }
            }

            &-2 {
                 background: url(https://colorlib.com/preview/theme/wines/images/wine_2.png) no-repeat center center;
            }

            &-3 {
                background: url(https://colorlib.com/preview/theme/wines/images/wine_3.png) no-repeat center center;
            }

            &-1,&-2,&-3 {
                 background-size: cover;
            }
            
        }
    }
</style>