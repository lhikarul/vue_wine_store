<template>
  <div class="intro">
      <div class="intro-item">
          <div class="img-wrapper">
              <img :src="img" alt="img" class="intro-item-img">
          </div>
            <div class="item-text-wrapper">
                <p class="item-text">
                    {{textOne}}
                </p>
                <p class="item-text">
                    {{textTwo}}
                </p>
            </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Intro',
    props: {
        img: {
            type: String,
            default: '',
            required: true
        },
        textOne: {
            type: String,
            default: '',
            required: true
        },
        textTwo: {
            type: String,
            default: '',
            required: true
        }        
    }
}
</script>

<style lang="scss" scoped>
    .intro {

        &-item {
            .img-wrapper {
                display: block;
                width: 100%;
            }

            &-img {
                width: 100%;
            }
        }

        .item-text-wrapper {
            padding: 30px;
            color: #8DA291;
            line-height: 1.5;

            .item-text:last-child {
                margin-top: 30px;
            }
        }
    }

    @media (min-width: 576px) {
        .intro {
            &-item {
                margin: 0 auto;
                max-width: 540px;
            }
        }
    }

    @media (min-width: 940px) {
        .intro {
            &-item {
                width: 100%;
                max-width: none;
                display: flex;

                .img-wrapper {
                    margin-top: -20px;

                    img {
                        display: block;
                        width: 460px;
                        height: 460px;
                    }
                }

                .item-text-wrapper {
                    box-sizing: border-box;
                    padding: 70px 35px;
                    height: 420px;
                    line-height: 2;
                    writing-mode: vertical-rl;

                    .item-text:last-child {
                        margin-top: 0;
                    }
                }
            }
        }
    }
</style>