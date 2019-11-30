<template>
  <div class="footer-area">
        <div class="my-container">
            <div class="img-wrapper">
                <img class="logo-img" src="https://colorlib.com/preview/theme/wines/images/logo.png" alt="logo">
            </div>

            <div class="footer-info">
                <div class="footer-info-phone">07-1234-5678</div>
                <div class="footr-info-email">wines@email.com</div>
                <div class="footer-info-address">800 高雄市新興區幸福路520號</div>
            </div>

            <div class="footer-bottom">

                <div class="social-icons">
                    <i class="fab fa-instagram"></i>
                    <i class="fab fa-facebook-square"></i>
                </div>

                <div class="copyright">© 1885 ~ 2019 wines* All Rights Reserved</div>

            </div>
        </div>
  </div>
</template>

<script>
export default {
    name: 'VFooter'
}
</script>

<style lang="scss" scoped>

    .my-container {
        margin: 0 auto;
        max-width: 940px;
    }

    .footer-area {
        padding: 30px;
        background: #EAF0ED;
        color: #3F5D45;

        .img-wrapper {
            margin-top: 9px;
        }

        .footer-info {
            margin-top: 39.5px;
            margin-bottom: 37px;
            line-height: 1.5;
        }

        .social-icons i {
            font-size: 32px;

            &:first-child {
                margin-right: 8px;
            }
        }

        .copyright {
            margin-top: 23px;
        }
    }

    @media (min-width: 940px) {
        .footer-area {
            .img-wrapper,.footer-info {
                text-align: center;
            }
            .footer-bottom {
                display: flex;
                justify-content: space-between;
                align-items: baseline;

                .copyright {
                    margin: 0;
                }
            }
        }
    }
</style>