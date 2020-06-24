<template>
    <div class="tags">
        <ul class="current">
            <li class="item-selected">
                <Icon name="personal"/>
                个人
            </li>
            <li>
                <Icon name="foods"/>
                餐饮
            </li>
            <li>
                <Icon name="drinks"/>
                饮料
            </li>
            <li>
                <Icon name="fruits"/>
                水果零食
            </li>
            <li>
                <Icon name="shopping"/>
                购物
            </li>
            <li>
                <Icon name="beauty"/>
                美容
            </li>
            <li>
                <Icon name="entertainment"/>
                娱乐
            </li>
            <li>
                <Icon name="movies"/>
                电影
            </li>
            <li>
                <Icon name="social"/>
                社交
            </li>
            <li>
                <Icon name="traffic"/>
                交通
            </li>

        </ul>
    </div>
</template>

<script lang="ts">
  export default {
    name: 'Tags'
  };
</script>

<style lang="scss" scoped>
    .tags {
        font-size: 12px;
        padding: 20px;
        flex-grow: 1;

        > .current {
            display: flex;
            flex-wrap: wrap;

            > li {
                display: flex;
                justify-content: center;
                align-items: center;
                flex-direction: column;
                padding: 10px 0;
                width: 20%;
                color: rgb(122, 135, 151);

                &.item-selected {
                    background: rgb(253, 245, 208);
                }
            }

            .icon {
                width: 2em;
                height: 2em;
                fill: rgb(122, 135, 151);
            }
        }
    }
</style>