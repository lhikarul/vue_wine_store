<template>
  <div class="pagination-container">
        <div class="pagination">
            <a href="javascript:;">&laquo;</a>
            <a href="javascript:;">1</a>
            <a href="javascript:;">2</a>
            <a href="javascript:;">3</a>
            <a href="javascript:;">&raquo;</a>
        </div>
  </div>
</template>

<script>
export default {
    name: 'Pagination'
}
</script>

<style lang="scss" scoped>
@import "styles/const";

    .pagination {
        display: inline-block;
        border: 1px solid $primary-light-color;

        a {
            float: left;
            width: 60px;
            height: 60px;
            line-height: 60px;
            color: $primary-color;
            font-size: 20px;
            text-align: center;
            text-decoration: none;

            &:nth-child(2) {
                background: $primary-color;
                color: $white;
            }
        }
    }

</style>