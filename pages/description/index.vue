<template>
    <Content :title="content.title" :part="content.part" :page="content.page">
        <AirlineDescription/>
    </Content>
</template>

<script>

    import Content from '@/components/Content';
    import AirlineDescription from '@/components/AirlineDescription';

    export default {
        data: function () {
            return {
                content: {
                    title: 'Сибирь',
                    part: 'Пассажирам',
                    page: 'Авиакомпании'
                }
            }
        },
        components: {
            Content,
            AirlineDescription
        }
    }

</script>

<style scoped>

</style>
