<template>
  <div>
        <VHeader></VHeader>
        <div class="banner"></div>
        <list></list>
        <heading-title subTitle="選擇了釀酒?"></heading-title>
        <intro
                img="http://www.xiangdu.com/Upload/2(8).jpg" 
                textOne="對酒當歌，人生幾何！譬如朝露，去日苦多。慨當以慷，憂思難忘。何以解憂？唯有杜康。青青子衿，悠悠我心。但為君故，沉吟至今。呦呦鹿鳴，食野之苹。我有嘉賓，鼓瑟吹笙。"
                textTwo="明明如月，何時可掇？憂從中來，不可斷絕。越陌度阡，枉用相存。契闊談宴，心念舊恩。月明星稀，烏鵲南飛。繞樹三匝，何枝可依？山不厭高，海不厭深。周公吐哺，天下歸心。"
        >
        </intro>
        <heading-title subTitle="一定要品酒?"></heading-title>
        <intro 
                img="https://article-picture.wine-world.com/c97be80a-efbf-4a69-b387-c46180c75c11.jpg"
                textOne="結廬在人境，而無車馬喧。問君何能爾？心遠地自偏。採菊東籬下，悠然見南山。"
                textTwo="山氣日夕佳，飛鳥相與還。此中有真意，欲辨已忘言。"
        >
        </intro>
        <heading-title title="品嘗美酒" subTitle="是不需要理由的"></heading-title>
        <item></item>

        <email></email>

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

    .banner {
        height: 277px;
        background: url(https://colorlib.com/preview/theme/wines/images/hero_1.jpg) no-repeat center center;
        background-size: cover;
    }
</style>