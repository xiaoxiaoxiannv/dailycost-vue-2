<template>
    <swiper class="swiper" :options="swiperOption">
        <swiper-slide>
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
        </swiper-slide>
        <swiper-slide>
            <div class="tags">
                <ul class="current">
                    <li class="item-selected">
                        <Icon name="App Store"/>
                        App Srote
                    </li>
                    <li>
                        <Icon name="phone"/>
                        手机通讯
                    </li>
                    <li>
                        <Icon name="computer"/>
                        电脑
                    </li>
                    <li>
                        <Icon name="present"/>
                        礼品
                    </li>
                    <li>
                        <Icon name="house"/>
                        居家
                    </li>
                    <li>
                        <Icon name="travel"/>
                        旅行
                    </li>
                    <li>
                        <Icon name="tickets"/>
                        门票
                    </li>
                    <li>
                        <Icon name="books"/>
                        书籍
                    </li>
                    <li>
                        <Icon name="medical"/>
                        医疗
                    </li>
                    <li>
                        <Icon name="transfer"/>
                        转账
                    </li>
                </ul>
            </div>
        </swiper-slide>
        <div class="swiper-pagination" slot="pagination">11111</div>
    </swiper>
</template>

<script lang="ts">
  import Vue from 'vue';
  import {Swiper, SwiperSlide} from 'vue-awesome-swiper';
  import 'swiper/swiper-bundle.css';
  import {Component} from 'vue-property-decorator';

  @Component({
    components: {
      Swiper,
      SwiperSlide,
    }
  })
  export default class Tags extends Vue {
    data() {
      return {
        swiperOption: {
          spaceBetween: 30,
          pagination: {
            el: '.swiper-pagination',
            clickable: true
          }
        }
      };
    }
  }
</script>

<style lang="scss" scoped>
    //@import '~@/assets/style/base.scss';
    .swiper {
        display: flex;
        flex-grow: 1;
        max-width: 100%;
        //justify-content: center;
        //align-items: center;
        //text-align: center;
        .tags {
            font-size: 12px;
            padding: 10px;
            position: relative;
            justify-content: center;
            align-items: center;

            > .current {
                display: flex;
                flex-wrap: wrap;

                > li {
                    display: flex;
                    //justify-content: center;
                    align-items: center;
                    flex-direction: column;
                    padding: 10px 10px;
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
    }
</style>