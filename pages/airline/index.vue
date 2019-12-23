<template>
    <Content :title="content.title" :part="content.part" :page="content.page">
        <AirlineGallery/>
    </Content>
</template>

<script>

    import Content from '@/components/Content';
    import AirlineGallery from '@/components/AirlineGallery';

    export default {
        data: function () {
          return {
              content: {
                  title: 'Авиакомпании',
                  part: 'Пассажирам',
                  page: 'Авиокомпании'
              }
          }
        },
        components: {
            Content,
            AirlineGallery
        }
    }

</script>

<style scoped>
</style>
