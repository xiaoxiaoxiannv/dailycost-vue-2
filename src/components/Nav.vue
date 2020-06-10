<template>
    <nav>
        <router-link to="/labels" class="item">
            <Icon name="label"/>
            标签
        </router-link>
        <router-link to="/money" class="item">
            <Icon name="money"/>
            记账
        </router-link>
        <router-link to="/statistics" class="item">
            <Icon name="statistics"/>
            账单
        </router-link>
    </nav>
</template>

<script lang="ts">
    export default {
    name: 'Nav'
  };
</script>

<style lang="scss" scoped>
    nav {
        display: flex;
        flex-direction: row;
        box-shadow: 0 0 3px rgba(0,0,0,0.25);
        font-size: 12px;
        >.item{
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            padding: 3px 0;
            width: 33.3333%;
            .icon{
                width: 32px;
                height: 32px;
            }
        }
    }
</style>