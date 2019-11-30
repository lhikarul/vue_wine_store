<template>
  <div class="home">
        <VHeader class="container"></VHeader>

        <div class="banner-area container">
            <div class="banner"></div>
            <list class="banner-list"></list>
        </div>

        <section class="section-intro mb-105 section-bg">
            
            <div class="container">

                <div class="home-intro-wrapper">

                    <heading-title class="home-title" subTitle="選擇了釀酒"></heading-title>

                    <intro  class="home-intro"
                            img="http://www.xiangdu.com/Upload/2(8).jpg" 
                            textOne="對酒當歌，人生幾何！譬如朝露，去日苦多。慨當以慷，憂思難忘。何以解憂？唯有杜康。青青子衿，悠悠我心。但為君故，沉吟至今。呦呦鹿鳴，食野之苹。我有嘉賓，鼓瑟吹笙。"
                            textTwo="明明如月，何時可掇？憂從中來，不可斷絕。越陌度阡，枉用相存。契闊談宴，心念舊恩。月明星稀，烏鵲南飛。繞樹三匝，何枝可依？山不厭高，海不厭深。周公吐哺，天下歸心。"
                    >
                    </intro>
                
                </div>

            </div>

        </section>

        <section class="section-intro section-bg">

            <div class="container">
                <div class="home-intro-wrapper">
                    
                    <heading-title class="home-title" subTitle="一定要品酒"></heading-title>

                    <intro  class="home-intro"
                            img="http://www.xiangdu.com/Upload/2(8).jpg"
                            textOne="結廬在人境，而無車馬喧。問君何能爾？心遠地自偏。採菊東籬下，悠然見南山。"
                            textTwo="山氣日夕佳，飛鳥相與還。此中有真意，欲辨已忘言。"
                    >
                    </intro>

                </div>
            </div>

        </section>

        <div class="heading">
            <heading-title class="heading-title" title="品嘗美酒" subTitle="是不需要理由的"></heading-title>
        </div>

        <div class="items-display-area">
            <div class="container">
                <div class="row">
                    <item class="item-display-area-item"></item>
                    <item class="item-display-area-item"></item>
                    <item class="item-display-area-item"></item>
                </div>
            </div>
        </div>

        <div class="email-area">
            <div class="container">
                 <email></email>
            </div>
        </div>

        <VFooter></VFooter>
  </div>
</template>

<script>
import VHeader from 'components/Header/Header';
import HeadingTitle from 'components/Home/Title';
import List from 'components/Home/List';
import Intro from 'components/Home/Intro';
import Item from 'components/Home/Item';
import Email from 'components/Home/Email';
import VFooter from 'components/Footer/Footer';

export default {
    name: "Home",
    components: {
        VHeader,
        HeadingTitle,
        List,
        Intro,
        Item,
        Email,
        VFooter
    }
}
</script>

<style lang="scss" scoped>

    .section-intro {
        margin: 30px 0;
    }

    .section-bg {
        background: #EAF0ED;
    }

    .banner {
        height: 277px;
        background: url(https://colorlib.com/preview/theme/wines/images/hero_1.jpg) no-repeat center center;
        background-size: cover;
    }

    .item-display-area {
        &-item:not(:last-child) {
            margin-bottom: 30px;
        }
    }

    .email-area {
        margin-top: 30px;
         background: #3F5D45;
    }

    @media (max-width: 939px) {
        .home-title {
            background: #fff;
        }
    }

    @media (min-width: 768px) {
        .banner {
            height: 496px;
        }
        .banner-list {
            margin-top: -105px;
        }
    }

    @media (min-width: 940px) {

        .row {
            display: flex;
        }

        .container {
            margin: 0 auto;
            max-width: 940px;
        }

        .mb-105 {
            margin-bottom: 105px;
        }

        .banner-area {
            margin-bottom: 80px;
        }

        .section-intro {
            height: 420px;

            .home-intro-wrapper {
                display: flex;
                flex-direction: row-reverse;
                position: relative;

                .home-title {
                    writing-mode: vertical-rl;
                }
            }

            .home-intro {
                flex: 1;
            }
        }

        .heading {
            margin-top: 95px;
            margin-bottom: 80px;
            &-title {
                margin: 0 auto;
                writing-mode: vertical-rl;
            }
        }

        .item-display-area {
            &-item:not(:last-child) {
                margin-bottom: 0px;
                margin-right: 20px;
            }
        }

        .email-area {
            margin-top: 60px;
        }
    }

</style>