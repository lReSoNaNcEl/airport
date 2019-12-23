<template>
    <Content :title="content.title" :part="content.part" :page="content.page">
        <PassengerInfo/>
    </Content>
</template>

<script>

    import Content from '@/components/Content';
    import PassengerInfo from '@/components/PassengerInfo';

    export default {
        data: function () {
            return {
                content: {
                    title: 'Информация для пассажиров',
                    part: 'Пассажирам',
                    page: 'Информация для пассажиров'
                }
            }
        },
        components: {
            Content,
            PassengerInfo
        }
    }

</script>

<style scoped>

</style>
