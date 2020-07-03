<template>
    <el-carousel indicator-position="outside">
        <el-carousel-item v-for="item in 4" :key="item">
            <h3>{{ item }}</h3>
<!--            <div class="container">-->
<!--                <div class="tags">-->
<!--                    <ul class="current">-->
<!--                        <li class="item-selected">-->
<!--                            <Icon name="personal"/>-->
<!--                            个人-->
<!--                        </li>-->
<!--                        <li>-->
<!--                            <Icon name="foods"/>-->
<!--                            餐饮-->
<!--                        </li>-->
<!--                        <li>-->
<!--                            <Icon name="drinks"/>-->
<!--                            饮料-->
<!--                        </li>-->
<!--                        <li>-->
<!--                            <Icon name="fruits"/>-->
<!--                            水果零食-->
<!--                        </li>-->
<!--                        <li>-->
<!--                            <Icon name="shopping"/>-->
<!--                            购物-->
<!--                        </li>-->
<!--                        <li>-->
<!--                            <Icon name="beauty"/>-->
<!--                            美容-->
<!--                        </li>-->
<!--                        <li>-->
<!--                            <Icon name="entertainment"/>-->
<!--                            娱乐-->
<!--                        </li>-->
<!--                        <li>-->
<!--                            <Icon name="movies"/>-->
<!--                            电影-->
<!--                        </li>-->
<!--                        <li>-->
<!--                            <Icon name="social"/>-->
<!--                            社交-->
<!--                        </li>-->
<!--                        <li>-->
<!--                            <Icon name="traffic"/>-->
<!--                            交通-->
<!--                        </li>-->

<!--                    </ul>-->
<!--                </div>-->
<!--                <ul class="dots">-->
<!--                    <li class="active"></li>-->
<!--                    <li></li>-->
<!--                </ul>-->
<!--            </div>-->
        </el-carousel-item>
    </el-carousel>
</template>

<script lang="ts">
  import Vue from 'vue';
  import {Component} from 'vue-property-decorator';

  @Component
  export default class Tags extends Vue {

  }
</script>

<style lang="scss" scoped>
    .el-carousel__item h3 {
        color: #475669;
        font-size: 18px;
        opacity: 0.75;
        line-height: 300px;
        margin: 0;
    }

    .el-carousel__item:nth-child(2n) {
        background-color: #99a9bf;
    }

    .el-carousel__item:nth-child(2n+1) {
        background-color: #d3dce6;
    }
    /*.container {*/
    /*    position: relative;*/
    /*    display: flex;*/
    /*    justify-content: center;*/
    /*    flex-grow: 1;*/

    /*    .tags {*/
    /*        font-size: 12px;*/
    /*        padding: 10px;*/
    /*        position: relative;*/
    /*        justify-content: center;*/
    /*        align-self: center;*/

    /*        > .current {*/
    /*            display: flex;*/
    /*            flex-wrap: wrap;*/

    /*            > li {*/
    /*                display: flex;*/
    /*                justify-content: center;*/
    /*                align-items: center;*/
    /*                flex-direction: column;*/
    /*                padding: 10px 10px;*/
    /*                width: 20%;*/
    /*                color: rgb(122, 135, 151);*/

    /*                &.item-selected {*/
    /*                    background: rgb(253, 245, 208);*/
    /*                }*/
    /*            }*/

    /*            .icon {*/
    /*                width: 2em;*/
    /*                height: 2em;*/
    /*                fill: rgb(122, 135, 151);*/
    /*            }*/
    /*        }*/
    /*    }*/

    /*    .dots {*/
    /*        display: flex;*/
    /*        position: absolute;*/
    /*        bottom: 10px;*/

    /*        > li {*/
    /*            width: 8px;*/
    /*            height: 8px;*/
    /*            border-radius: 50%;*/
    /*            background: rgb(211, 216, 220);*/
    /*            margin: 0 5px;*/

    /*            &.active {*/
    /*                background: rgb(122, 135, 151);*/
    /*            }*/
    /*        }*/
    /*    }*/
    /*}*/
</style>