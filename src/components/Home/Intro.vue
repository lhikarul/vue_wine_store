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
                max-width: 375px;
                width: 100%;
            }

            &-img {
                width: 100%;
            }
        }

        .item-text-wrapper {
            padding: 30px;
            background: #EAF0ED;
            color: #8DA291;
            line-height: 1.5;

            .item-text:last-child {
                margin-top: 30px;
            }
        }

    }
</style>