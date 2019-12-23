<template>
    <div class="content">
        <h1 class="content__title">{{mainTitle}}</h1>
        <p class="content__text">
            <span>{{part}}</span> → {{page}}
        </p>
        <slot></slot>
    </div>
</template>

<script>
    export default {
        props: {
            title: String,
            part: String,
            page: String
        },
        data: function () {
            return {
                mainTitle: null
            }
        },
        mounted() {
            if (this.$route.query.title !== undefined) {
                this.mainTitle = this.$route.query.title;
            }
            else {
                this.mainTitle = this.title;
            }
        }
    }

</script>

<style scoped>
    .content {
        margin: 0 0 0 13.8vw;
    }

    .content__title {
        font-size: 1.5625vw;
        color: #424242;
        line-height: 1.5625vw;
        font-weight: 500;
        margin: 2.34375vw 0 1.0416vw 0;
    }

    .content__text {
        font-size: 0.9375vw;
        color: #949494;
        margin: 0 0 1.5625vw 0;
    }

    .content__text > span {
        color: #38A0F2;
    }

</style>
