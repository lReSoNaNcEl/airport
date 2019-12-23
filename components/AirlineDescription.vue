<template>
     <div>
         <div class="content__company">
             <div class="flex-wrap">
                 <div ref="picture" class="content__company__image"></div>
                 <div ref="about" class="content__company__about">
                     {{this.slides[0].text}}
                 </div>
             </div>
             <div class="content__slider" ref="slides">
                 <div data-image="utair" class="content__slider__item slide"></div>
                 <div data-image="orenburg" class="content__slider__item slide"></div>
                 <div data-image="yamal" class="content__slider__item slide"></div>
                 <div data-image="rusline" class="content__slider__item slide"></div>
                 <div data-image="siberia" class="content__slider__item slide"></div>
             </div>
         </div>
     </div>
</template>

<script>

    export default {

        props: {
            company: String

        },
        data: function () {
            return {
                slides: [
                    {
                        value: 'utair',
                        title: 'ЮТэйр',
                        src: '_nuxt/assets/img/airline/ЮТэйр.png',
                        text: 'Российская авиакомпания, выполняющая внутренние и международные пассажирские авиаперевозки. Вместе с авиакомпанией Глобус образует холдинг S7 Group, специализирующийся на продаже авиабилетов и пакетных туров, подготовке лётного персонала, ремонте воздушных судов и других авиационных услугах. Сама S7 Airlines является 2-й в стране крупнейшей авиакомпанией, обслужившей за 2016 год свыше 9,5 миллионов пассажиров, уступая по этому показателю лишь национальному перевозчику Аэрофлоту.'
                    },
                    {
                        value: 'orenburg',
                        title: 'Оренбуржье',
                        src: '_nuxt/assets/img/airline/Оренбуржье.png',
                        text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Facilis illum inventore sequi temporibus veniam veritatis. Ex incidunt quasi totam voluptas.'
                    },
                    {
                        value: 'yamal',
                        title: 'Ямал',
                        src: '_nuxt/assets/img/airline/Ямал.png',
                        text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. A adipisci amet culpa dicta dolore ipsam, molestias, nam nostrum omnis pariatur quaerat sunt velit vero voluptatem?'
                    },
                    {
                        value: 'rusline',
                        title: 'Руслайн',
                        src: '_nuxt/assets/img/airline/Руслайн.png',
                        text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci atque doloribus explicabo fugit harum inventore iure nam nemo nihil sunt. Amet, aut tempora!'
                    },
                    {
                        value: 'siberia',
                        title: 'Сибирь',
                        src: '_nuxt/assets/img/airline/Сибирь.png',
                        text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias architecto aspernatur at delectus eaque ipsum quas saepe veniam.'
                    }
                ],
                activeCompany: null
            }
        },
        components: {

        },
        methods: {
          setActiveCompany: function (company, picture, text, images) {

              for (let airline of this.slides) {
                  console.log(airline.value);
                  if (airline.value === company) {
                      document.querySelector('.content__title').textContent = airline.title;
                      picture.style.backgroundImage = `url('${airline.src}')`;
                      text.textContent = airline.text;
                  }
              }

              for (let image of images) {
                  image.classList.remove('active');
                  if (image.getAttribute('data-image') === company)
                      image.classList.add('active');
              }
          }
        },
        mounted: function () {
            this.activeCompany = this.$route.query.company;

            const picture = this.$refs.picture;
            const text = this.$refs.about;
            const slides = this.$refs.slides.children;
            let images = [];

            for (let i = 0; i <= slides.length - 1; i++) {
                images[i] = slides[i];
            }
            this.setActiveCompany(this.activeCompany, picture, text, images);

            if (this.activeCompany === undefined) {
                document.getElementsByClassName('content__slider__item')[0].classList.add('active');
                picture.style.backgroundImage = `url('${this.slides[0].src}')`;
            }

            for (let image of images) {
                image.addEventListener('click', (e) => {
                    this.activeCompany = e.target.getAttribute('data-image');
                    this.setActiveCompany(this.activeCompany, picture, text, images);
                    e.target.classList.add('active');
                });
            }
        }
    }

</script>

<style scoped>
    .flex-wrap {
        display: flex;
        height: 28.64583vw;
    }

    .content__company__image {
        background: url('../assets/img/airline/Сибирь.png');
        background-position: 50%;
        width: 35.9375vw;
        height: 17.96875vw;
        background-size: cover;
    }

    .content__company__about {
        position: relative;
        z-index: 1;
        width: 41.6vw;
        height: 18.22916vw;
        background-color: white;
        right: 5.2083vw;
        top: 7.8125vw;
        padding: 2.083vw;
        line-height: 1.875vw;
        font-size: 1.0416vw;
        color: #333333;
    }

    .content__slider {
        display: flex;
        flex-wrap: wrap;
        width: 100%;
    }


    .content__slider__item {
        width: 13.02083vw;
        height: 5.2083vw;
        background-size: cover;
        background-repeat: no-repeat;
        background-position: 50%;
        margin: 0 1.302vw 1.416vw 0;
    }

    .content__slider__item:hover {
        cursor: pointer;
    }

    .content__slider__item:nth-of-type(1) {background: url('../assets/img/airline/ЮТэйр.png');}
    .content__slider__item:nth-of-type(2) {background: url('../assets/img/airline/Оренбуржье.png');}
    .content__slider__item:nth-of-type(3) {background: url('../assets/img/airline/Ямал.png');}
    .content__slider__item:nth-of-type(4) {background: url('../assets/img/airline/Руслайн.png');}
    .content__slider__item:nth-of-type(5) {background: url('../assets/img/airline/Сибирь.png');}

    .content__slider__item:nth-of-type(1)::before {content: "ЮТейр";}
    .content__slider__item:nth-of-type(2)::before {content: "Оренбуржье";}
    .content__slider__item:nth-of-type(3)::before {content: "Ямал";}
    .content__slider__item:nth-of-type(4)::before {content: "Руслайн";}
    .content__slider__item:nth-of-type(5)::before {content: "Сибирь";}

    .content__slider__item:nth-of-type(1n)::before {
        display: block;
        color: white;
        font-size: 1.40625vw;
        font-weight: 500;
        margin: 1.822916vw 0 0 1.302083vw;
    }

    .active {
        height: 6.77083vw;
        position: relative;
        bottom: 0.78125vw;
    }

    .content__slider__item.active::before {
        margin: 2.5vw 0 0 1.302083vw;
    }


</style>
