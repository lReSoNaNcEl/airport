<template>
    <div class="container">
        <button ref="btn" @click="toggleVisibleDescription()" class="container__toggle">{{title}}</button>
        <div ref="info" class="container__info">
            <p class="container__info__item" v-for="proposal in text">{{proposal}}</p>
        </div>
    </div>
</template>

<script>
    export default {
        data: function () {
            return {
                text: this.description.match(/[^\.!\?]+/g)
            }
        },
        props: {
            title: String,
            description: String
        },
        methods: {
            toggleVisibleDescription: function () {
                const btn = this.$refs.btn;
                const info = btn.nextElementSibling;

                btn.classList.toggle('active');

                if (btn.classList.contains('active')) {
                    info.style.display = 'block';
                }
                else {
                    info.style.display = 'none';
                    btn.classList.remove('active');
                }
            }
        }
    }
</script>

<style scoped>

    .container {
        border: 1px solid #BBBBBB;
        border-radius: 10px;
        width: 52vw;
        margin: 0 0 20px 0;
    }

    .container__toggle {
        padding: 0 60% 0 0;
        border-radius: 10px;
        margin: 1.0416vw 0 1.302083vw 1.302083vw;
        color: #38A0F2;
        font-weight: 500;
        font-size: 1.0415vw;
        background-color: white;
        border: none;
        outline: none;
    }

    .container__toggle:hover {
        cursor: pointer;
    }

    .container__info {
        display: none;
        color: #615E5E;
        line-height: 1.302083vw;
        margin: 0 3.125vw 0 4.16vw;
    }

    .container__info__item {
        margin: 0 0 1.5625vw 0;
        font-size: 1.0415vw;
    }
</style>
