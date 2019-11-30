<template>
  <div class="email-area">
        <div class="email-wrapper">
            <div class="email-info-wrapper">
                <div class="img-wrapper">
                    <img src="https://previews.123rf.com/images/topvectors/topvectors1712/topvectors171200354/91202652-wine-label-%C3%B1%C6%92%C3%B1%E2%80%B9%C3%B0%C2%B5%C3%B0%C2%B2-1935-natural-top-quality-product-vintage-logo-design-element-for-menu-winery-log.jpg" alt="brand logo">
                </div>
                <h3 class="email-info-text">訂閱你我的甜蜜郵件</h3>
            </div>
            <div class="input-wrapper">
                <span><i class="fas fa-envelope"></i></span>
                <input class="email" type="email" />
                <span class="icon-arrow"><i class="fas fa-arrow-right"></i></span>
            </div>
        </div>
  </div>
</template>

<script>
export default {
    name: 'Email'
}
</script>

<style lang="scss" scoped>
    .email-area {

        padding: 30px;

        .email-info-wrapper {
            
            padding: 0 20px;
            display: flex;
            align-items: center;
            justify-content: center;

            .img-wrapper img {
                border-radius: 50%;
                width: 40px;
                height: 40px;
            }

            .email-info-text {
                padding-left: 20px;
                color: #EAF0ED;
            }
        }

        .input-wrapper {
            margin-top: 30px;
            padding-left: 20px;
            display: flex;
            align-items: center;
            height: 56px;
            line-height: 56px;
            background: #EAF0ED;

            input.email {
                flex: 1;
                margin-left: 20px;
                border: none;
                background: transparent;
                outline: none;
            }

            .icon-arrow {
                flex-basis: 64px;
                width: 64px;
                background: #FFE180;
                color: #3F5D45;
                text-align: center;
            }
        }
    }

    @media (min-width: 940px) {
        .email-area {
            .email-wrapper {
                padding: 0 15%;
                display: flex;
                justify-content: space-between;
                align-items: center;

                .email-info-wrapper {
                    padding: 0;

                    .email-info-text {
                        font-size: 24px;
                    }
                }

                .input-wrapper {
                    margin-top: 0;
                }
            }
        }
    }
</style>