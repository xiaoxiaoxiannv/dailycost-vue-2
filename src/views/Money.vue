<template>
    <Layout class-prefix="layout">
        <NumberPad/>
        <Notes/>
        <Tags :data-source="tags"/>
        <Types/>
    </Layout>
</template>

<script>
    import NumberPad from '@/components/Money/NumberPad.vue';
    import Notes from '@/components/Money/Notes.vue';
    import Tags from '@/components/Money/Tags.vue';
    import Types from '@/components/Money/Types.vue';
    //import Item from '@/components/Money/Tags.vue';

    export default {
        name: 'Money',
        components: {Types, Tags, Notes, NumberPad},
        data() {
            return {
                tags: [
                    {icon: 'personal', name: '个人'},
                    {icon: 'foods', name: '餐饮'},
                    {icon: 'drinks', name: '饮料'},
                    {icon: 'fruits', name: '水果零食'},
                    {icon: 'shopping', name: '购物'},
                    {icon: 'beauty', name: '美容'},
                    {icon: 'entertainment', name: '娱乐'}],
            }
        }
    };
</script>

<style lang="scss">
    .layout-content {
        display: flex;
        flex-direction: column-reverse;
    }
</style>
