<template>
    <div class="content">
        <div class="content__toggle">
            <div class="content__toggle__item">
                <div class="content__toggle__item__text">Вылет</div>
                <svg width="31" height="24" viewBox="0 0 31 24" xmlns="http://www.w3.org/2000/svg">
                    <path d="M4.23165 13.7068C3.97193 13.8289 3.8543 14.1428 3.96622 14.4135L5.11511 17.044C5.17154 17.175 5.27607 17.2777 5.40551 17.3292C5.46223 17.3513 5.52252 17.363 5.58326 17.3637C5.65927 17.3653 5.73449 17.3494 5.80399 17.3178L14.7668 13.1208L13.8572 21.833C13.8396 22.0045 13.9017 22.1741 14.0246 22.2902C14.4114 22.629 14.8961 22.8251 15.4026 22.8481C15.5423 22.8496 15.6814 22.8331 15.8172 22.799C16.543 22.6124 17.1118 21.9528 17.5079 20.8195L21.141 10.1292L28.1265 6.86252C30.1827 5.9007 31.2598 3.91412 30.5706 2.34558C30.1786 1.52537 29.4159 0.961606 28.538 0.842547C27.563 0.678743 26.5628 0.825817 25.6703 1.26429L17.6088 5.05429L9.03119 1.46981C7.95079 1.03466 7.09105 1.03543 6.48293 1.47809C5.97207 1.90102 5.67671 2.5423 5.68109 3.21849C5.68434 3.39006 5.76604 3.54966 5.90148 3.64932L11.6565 7.83982L8.31389 9.42603L2.758 7.89778C2.53032 7.83708 2.29135 7.94066 2.17312 8.15102L0.753726 10.7186C0.680048 10.8547 0.666813 11.0171 0.717468 11.1639C0.767794 11.3109 0.877087 11.4281 1.01746 11.4857L5.12265 13.2949L4.23165 13.7068ZM6.75879 2.96034C6.79234 2.73168 6.90692 2.5245 7.08038 2.37892C7.38194 2.16019 7.92678 2.19916 8.65208 2.48932L16.2909 5.67271L12.7689 7.32181L6.75879 2.96034ZM1.94897 10.7274L2.88077 9.06417L8.22769 10.5029C8.34292 10.5345 8.46503 10.5246 8.57431 10.4748L26.1044 2.26619C26.8015 1.92112 27.5835 1.80169 28.3472 1.92399C28.8831 1.98135 29.3573 2.30691 29.6164 2.79486C30.0449 3.77532 29.1634 5.18987 27.6923 5.87691L21.6187 8.73159L21.9989 7.6142C22.0951 7.32672 21.9472 7.01313 21.6691 6.91417C21.3906 6.81521 21.0872 6.96826 20.9912 7.25574L16.5209 20.4718C16.2551 21.222 15.93 21.668 15.5724 21.761C15.3511 21.8024 15.1231 21.7549 14.9343 21.6292L16.1163 10.265C16.1473 9.96622 15.9381 9.69823 15.6487 9.6665C15.3596 9.63443 15.1001 9.85111 15.069 10.1499L14.8862 11.8868L5.83895 16.1151L5.11924 14.4812L6.60569 13.7836C6.79698 13.6992 6.9219 13.5062 6.92442 13.2916C6.92694 13.0768 6.80658 12.881 6.61732 12.7922L1.94897 10.7274Z" fill="#38A0F2"/>
                </svg>
            </div>
            <div class="content__toggle__item content__toggle__item_active">
                <div class="content__toggle__item__text">Прилет</div>
                <svg width="38" height="38" viewBox="0 0 38 38" xmlns="http://www.w3.org/2000/svg">
                    <path d="M9.63701 12.897C9.36318 12.811 9.06407 12.9623 8.96308 13.2373L8.02707 15.9508C7.9799 16.0854 7.98727 16.2318 8.04759 16.3574C8.0744 16.412 8.11081 16.4614 8.15502 16.5031C8.20988 16.5557 8.27601 16.595 8.34854 16.6188L17.7856 19.6003L11.2164 25.3948C11.0873 25.509 11.0181 25.6758 11.0299 25.8445C11.0851 26.3557 11.309 26.8282 11.666 27.1882C11.7678 27.2839 11.8813 27.3659 12.0044 27.4329C12.6648 27.7871 13.53 27.6869 14.5889 27.1212L24.5017 21.7157L31.8537 24.0427C34.018 24.7274 36.1559 23.9951 36.7109 22.3742C36.9779 21.5052 36.7986 20.5739 36.2333 19.8918C35.6267 19.111 34.7912 18.5419 33.8376 18.2601L25.3393 15.5895L21.4554 7.14334C20.9551 6.09151 20.322 5.50986 19.5748 5.42374C18.9125 5.38899 18.2609 5.66082 17.8062 6.16132C17.6924 6.28976 17.6444 6.46252 17.6766 6.62757L19.0733 13.6082L15.5396 12.5118L12.4865 7.62482C12.3601 7.42597 12.1141 7.34035 11.8847 7.41507L9.10153 8.34308C8.95518 8.3933 8.83547 8.50382 8.7733 8.64618C8.71077 8.78843 8.71184 8.94866 8.77609 9.08612L10.5715 13.1973L9.63701 12.897ZM18.774 6.70119C18.9535 6.55567 19.1781 6.48082 19.4043 6.49117C19.7743 6.53445 20.1488 6.93209 20.486 7.63676L23.9509 15.1521L20.2426 13.9804L18.774 6.70119ZM9.97506 9.15895L11.787 8.56619L14.7469 13.2458C14.8103 13.347 14.9069 13.4224 15.021 13.4598L33.4785 19.2913C34.2251 19.5095 34.8814 19.9512 35.3605 20.5583C35.716 20.9635 35.8444 21.5241 35.7046 22.0586C35.356 23.0703 33.7494 23.5141 32.2017 23.0234L25.7995 21.0108L26.836 20.4461C27.1014 20.2997 27.205 19.9688 27.0674 19.7077C26.9295 19.4463 26.6026 19.3534 26.3373 19.4999L14.0981 26.197C13.3945 26.569 12.8533 26.677 12.5272 26.5033C12.3363 26.3839 12.2007 26.1945 12.1469 25.9741L20.7125 18.4129C20.9376 18.214 20.9652 17.8752 20.7737 17.6558C20.5827 17.4364 20.245 17.4201 20.0198 17.6189L18.7091 18.7732L9.18875 15.7575L9.76565 14.0679L11.3318 14.5613C11.5297 14.6287 11.7523 14.5713 11.8995 14.4151C12.0468 14.2588 12.0909 14.0331 12.0117 13.8397L9.97506 9.15895Z" fill="white"/>
                </svg>
            </div>
        </div>

        <div class="content__dashboard">
            <h2 class="content__dashboard__title">Расписание на</h2>
            <div class="content__dashboard__btn content__dashboard__btn_active">Сегодня</div>
            <div class="content__dashboard__btn">Завтра</div>
            <div class="content__dashboard__btn">На неделю</div>
        </div>

        <hr>

        <div class="content__timetable">
            
            <div class="content__timetable__title">
                <div class="content__timetable__title__item">Дата</div>
                <div class="content__timetable__title__item">Время</div>
                <div class="content__timetable__title__item">Рейс</div>
                <div class="content__timetable__title__item">Направление</div>
                <div class="content__timetable__title__item">Авиакомпания</div>
                <div class="content__timetable__title__item">Самолет</div>
                <div class="content__timetable__title__item">Статус</div>
            </div>

            <div v-for="item in timetable" :key="item.id">
                <hr class="content__timetable__line-split">
                <div class="content__timetable__item">
                    <div class="content__timetable__item__data">{{item.date}}</div>
                    <div class="content__timetable__item__data">{{item.time}}</div>
                    <div class="content__timetable__item__data">{{item.flight}}</div>
                    <div class="content__timetable__item__data">{{item.direction}}</div>
                    <div class="content__timetable__item__data">{{item.airline}}</div>
                    <div class="content__timetable__item__data">{{item.airplane}}</div>
                    <div class="content__timetable__item__data">{{item.status}}</div>
                </div>
            </div>

        </div>

    </div>
</template>

<script>
    export default {
        data: function () {
            return {
                timetable: [
                    {
                        id: 1,
                        date: '25.10',
                        time: '10:15',
                        flight: 'S7284',
                        direction: 'Москва(Домодедово)',
                        airline: 'Сибирь',
                        airplane: 'EMB-170',
                        status: 'Регистрация в 8:15'
                    },
                    {
                        id: 2,
                        date: '25.10',
                        time: '10:15',
                        flight: 'S7284',
                        direction: 'Москва(Домодедово)',
                        airline: 'Сибирь',
                        airplane: 'EMB-170',
                        status: 'Регистрация в 8:15'
                    },
                    {
                        id: 3,
                        date: '25.10',
                        time: '10:15',
                        flight: 'S7284',
                        direction: 'Москва(Домодедово)',
                        airline: 'Сибирь',
                        airplane: 'EMB-170',
                        status: 'Регистрация в 8:15'
                    },
                    {
                        id: 4,
                        date: '25.10',
                        time: '10:15',
                        flight: 'S7284',
                        direction: 'Москва(Домодедово)',
                        airline: 'Сибирь',
                        airplane: 'EMB-170',
                        status: 'Регистрация в 8:15'
                    },
                    {
                        id: 5,
                        date: '25.10',
                        time: '10:15',
                        flight: 'S7284',
                        direction: 'Москва(Домодедово)',
                        airline: 'Сибирь',
                        airplane: 'EMB-170',
                        status: 'Регистрация в 8:15'
                    },
                    {
                        id: 6,
                        date: '25.10',
                        time: '10:15',
                        flight: 'S7284',
                        direction: 'Москва(Домодедово)',
                        airline: 'Сибирь',
                        airplane: 'EMB-170',
                        status: 'Регистрация в 8:15'
                    },
                    {
                        id: 7,
                        date: '25.10',
                        time: '10:15',
                        flight: 'S7284',
                        direction: 'Москва(Домодедово)',
                        airline: 'Сибирь',
                        airplane: 'EMB-170',
                        status: 'Регистрация в 8:15'
                    },
                    {
                        id: 8,
                        date: '25.10',
                        time: '10:15',
                        flight: 'S7284',
                        direction: 'Москва(Домодедово)',
                        airline: 'Сибирь',
                        airplane: 'EMB-170',
                        status: 'Регистрация в 8:15'
                    },
                    {
                        id: 9,
                        date: '25.10',
                        time: '10:15',
                        flight: 'S7284',
                        direction: 'Москва(Домодедово)',
                        airline: 'Сибирь',
                        airplane: 'EMB-170',
                        status: 'Регистрация в 8:15'
                    },
                    {
                        id: 10,
                        date: '25.10',
                        time: '10:15',
                        flight: 'S7284',
                        direction: 'Москва(Домодедово)',
                        airline: 'Сибирь',
                        airplane: 'EMB-170',
                        status: 'Регистрация в 8:15'
                    },
                ]
            }
        }
    }

</script>

<style scoped>
    .content {
        width: 72.5vw;
        margin: 0 0 0 13.8vw;
    }

    .content__toggle,
    .content__toggle__item,
    .content__dashboard,
    .content__timetable__title,
    .content__timetable__item {
        display: flex;
    }

    .content__toggle {
        justify-content: space-evenly;
        width: 16.6vw;
        height: 2.34375vw;
        border-radius: 100px;
        border: 1px solid #38A0F2;
        margin: 0 0 1.5625vw 0;
    }

    .content__toggle__item {
        width: 50%;
        justify-content: center;
        align-items: center;
        font-size: 1.14583vw;
        stroke: #38A0F2;
        stroke-width: .7;
    }

    .content__toggle__item.content__toggle__item_active > svg {stroke: white;}

    .content__toggle__item:first-child {border-radius: 100px 0 0 100px;}
    .content__toggle__item:last-child {border-radius: 0 100px 100px 0;}

    .content__toggle__item:hover {cursor: pointer;}

    .content__toggle__item__text {margin: 0 .52083vw 0 0;}

    .content__dashboard {
        align-items: center;
        width: 35.9375vw;
        justify-content: space-between;
    }

    .content__dashboard__title {
        font-size: 1.5625vw;
        font-weight: 500;
        color: #5B5B5B;
    }

    .content__dashboard__btn {font-size: 1.14583vw;}

    .content__dashboard__btn:hover {cursor: pointer;}

    .content__timetable__line-split {
        background-color: #EDEDED;
        height: 1px;
        border: none;
    }

    .content__timetable__title {
        margin: 1.5625vw 0 1.302083vw 0;
    }

    .content__timetable__title__item {
        font-weight: 500;
        font-size: 1.14583vw;
    }

    .content__timetable__title__item:nth-of-type(-n+3),
    .content__timetable__item__data:nth-of-type(-n+3){width: 8.85416vw;}

    .content__timetable__title__item:nth-of-type(4),
    .content__timetable__item__data:nth-of-type(4){width: 15.625vw;}

    .content__timetable__title__item:nth-of-type(5),
    .content__timetable__item__data:nth-of-type(5){width: 12.5vw;}

    .content__timetable__title__item:nth-of-type(6),
    .content__timetable__item__data:nth-of-type(6){width: 8.3vw;}

    .content__timetable__title__item:nth-of-type(7),
    .content__timetable__item__data:nth-of-type(7){width: 10.416vw;}

    .content__timetable__item {
        margin: 1.5625vw 0 1.5625vw 0;
    }

    .content__timetable__item__data {
        font-size: 1.0416vw;
        color: #333333;
    }

    .content__toggle__item_active {
        background-color: #38A0F2;
        color: white;
    }

    .content__dashboard__btn_active {
        background-color: #38A0F2;
        color: white;
        padding: .625vw 1.5625vw .625vw 1.5625vw;
        border-radius: 18px 18px 0 0;
    }

</style>