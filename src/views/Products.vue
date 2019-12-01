<template>
  <div>
      <div class="banner-area">
          <div class="container">
              <div class="banner"></div>
          </div>
      </div>

        <div class="items-display-area">
            <div class="container">
                <div class="row">

                    <div class="column-md-4">
                        <types></types>
                    </div>
                    
                    <div class="column-md-8">
                        <items></items>
                    </div>
                </div>
            </div>
        </div>

        <div class="pagination-area">
            <pagination></pagination>
        </div>

      <div class="email-area full-background">
          <email></email>
      </div>

  </div>
</template>

<script>
import Types from 'components/Products/Types';
import Items from 'components/Products/Items';
import Pagination from 'base/Pagination';
import Email from 'base/Email';

export default {
    name: "Products",
    components: {
        Types,
        Items,
        Pagination,
        Email
    }
}
</script>

<style lang="scss" scoped>
@import 'styles/const';

// ----- grid ----- //

    @media (min-width: 940px) {
        .row {
            display: flex;
            flex-wrap: wrap;
        }
        
        .column-md-4 {
            flex: 0 0 33.33333%;
            max-width: 0 0 33.33333%;
        }

        .column-md-8 {
            flex: 0 0 66.66666%;
            max-width: 66.66666%;
        }
    }

// ----- end of gird ----- //

    .container {
        margin: 0 auto;
        max-width: 940px;
    }

    .full-background {
        background-color: $primary-color;
    }

    .banner-area {
        .banner {
            height: 277px;
            background: url(https://www.abelandcole.co.uk/media/6347_27088_z.jpg) no-repeat center center;
            background-size: cover;

            @media (min-width: 768px) {
                height: 496px;
            }
        }
    }

    .items-display-area {
        margin-bottom: 30px;

        @media (min-width: 940px) {
            margin-top: 60px;
        }
    }

    .pagination-area {
        text-align: center;
        @media (min-width: 940px) {
            text-align: right;
        }
    }

    .email-area {
        margin-top: 30px;
        @media (min-width: 940px) {
            margin-top: 60px;
        }
    }

</style>