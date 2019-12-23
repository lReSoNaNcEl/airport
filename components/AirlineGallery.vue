<template>
    <div>
        <div ref="slides" class="content__images">
            <div data-image="utair" class="content__images__img"></div>
            <div data-image="orenburg" class="content__images__img"></div>
            <div data-image="yamal" class="content__images__img"></div>
            <div data-image="rusline" class="content__images__img"></div>
            <div data-image="siberia" class="content__images__img"></div>
        </div>
    </div>
</template>

<script>

    import Content from '@/components/Content';

    export default {
        data: function () {
          return {
              company: null,
              titles: [
                  'ЮТэйр',
                  'Оренбуржье',
                  'Ямал',
                  'Руслайн',
                  'Сибирь',
              ],
              titleDescription: null
          }
        },
        components: {
            Content
        },
        mounted: function () {
            console.log(this.$root.title);


            let images = [];
            const slides = this.$refs.slides.children;

            for (let i = 0; i <= slides.length - 1; i++) {
                images[i] = slides[i];
            }

            for (let image of images) {
                image.addEventListener('click', (e) => {
                    this.company = e.target.getAttribute('data-image');

                    switch (this.company) {
                        case 'utair': this.titleDescription = this.titles[0]; break;
                        case 'orenburg': this.titleDescription = this.titles[1]; break;
                        case 'yamal': this.titleDescription = this.titles[2]; break;
                        case 'rusline': this.titleDescription = this.titles[3]; break;
                        case 'siberia': this.titleDescription = this.titles[4]; break;
                    }

                    this.$router.push({name: 'description', query: {company: this.company, title: this.titleDescription}})
                });
            }

        }
    }

</script>

<style scoped>

    .content__images {
        display: flex;
        flex-wrap: wrap;
    }

    .content__images__img {
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
        width: 35.416vw;
        height: 25.260416vw;
        margin: 0 1.302vw 1.416vw 0;
    }

    .content__images__img:hover {
        filter: grayscale(30%);
        transition: .3s;
        cursor: pointer;
    }

    .content__images__img:nth-of-type(1) {background: url('../assets/img/airline/ЮТэйр.png');}
    .content__images__img:nth-of-type(2) {background: url('../assets/img/airline/Оренбуржье.png');}
    .content__images__img:nth-of-type(3) {background: url('../assets/img/airline/Ямал.png');}
    .content__images__img:nth-of-type(4) {background: url('../assets/img/airline/Руслайн.png');}
    .content__images__img:nth-of-type(5) {background: url('../assets/img/airline/Сибирь.png');}

    .content__images__img:nth-of-type(1)::before {content: "ЮТейр";}
    .content__images__img:nth-of-type(2)::before {content: "Оренбуржье";}
    .content__images__img:nth-of-type(3)::before {content: "Ямал";}
    .content__images__img:nth-of-type(4)::before {content: "Руслайн";}
    .content__images__img:nth-of-type(5)::before {content: "Сибирь";}

    .content__images__img:nth-of-type(1n)::before {
        display: block;
        color: white;
        font-size: 2.083vw;
        font-weight: 500;
        margin: 3.6458vw 0 0 2.60416vw;
        width: 20%;
    }
    .content__images__img:nth-of-type(1n):hover::before {
        opacity: .8;
        transition: .6s;
    }
</style>
