<template>
    <a-carousel :after-change="onChange">
        <div><h3>1</h3></div>
        <div><h3>2</h3></div>
        <div><h3>3</h3></div>
        <div><h3>4</h3></div>
    </a-carousel>
</template>

<script lang="ts">
    import Vue from 'vue';
    import {Component} from 'vue-property-decorator';

    @Component
    export default class Tags extends Vue{
      onChange(a, b, c) {
        console.log(a, b, c);
      }
    }
</script>

<style lang="scss" scoped>
    .ant-carousel {
        .slick-slide {
            text-align: center;
            height: 160px;
            line-height: 160px;
            background: #364d79;
            overflow: hidden;
            >h3 {
                color: #fff;
            }
        }
    }
</style>