<template>
<v-container grid-list-sm>
<v-layout row wrap>
    <v-flex col-sm-6 class="title">
        <h2 class="text-first">БЕСПЛАТНЫЙ онлайн-вебинар</h2>
        <h2 class="text-first" style="color:yellow;">ЕВРЕЙСКАЯ ЭМИГРАЦИЯ</h2>
        <h2 class="text-first" style="color:yellow;">в ГЕРМАНИЮ</h2>
        <h2 class="text-second">Вопросы руководителю русскоязычного общества Германии</h2>
        <h2 class="text-third">
            <span class="title-number">25</span>
            сентября / четверг /
            <span class="title-number">19-00</span> 
            <span style="font-size: 30px; letter-spacing: 0px; font-weight: 300; margin-left: 4px"> (киевское)</span> 
        </h2>
    </v-flex>
    <v-flex col-sm-6 class="counter">
        <span class="number">{{ this.number }} </span>
        <h3 class="text-number">мест осталось</h3>
    </v-flex>
</v-layout>
<v-layout align-center justify-center column >
        <button class="button" v-on:click="newnumber" >ЗАРЕГИСТРИРОВАТЬСЯ</button>
        <p class="under-button">Запись предоставляется бесплатно только зарегистрированным участникам</p>
        <span class="icon-стрелка"></span>
</v-layout>
</v-container>
</template>

<script>
export default {
    data() {
        return{
            number: 99,
        }      
    },
    methods: {
        newnumber () {
            this.number = this.number - 1
        }
    }
    }
    

</script>

<style scoped>

.counter{
    margin-top: 144px;
    margin-bottom: 23px;
    margin-right: 147px;
    border: 2px solid white;
    max-width: 365px;
    text-align: center;
}

.title {
    margin-top: 129px;
    margin-left: 141px;
}

.title-number{
    font-size: 60px;
    font-weight:400;
}
.text-first{
    letter-spacing: 0px;
    /* Style for "БЕСПЛАТНЫЙ" */
    font-size: 70px;
    font-weight: 700;
    line-height: 77px;
    /* Text style for "БЕСПЛАТНЫЙ" */
    color: #ffffff;
    font-family: "Roboto";
    text-align: left;
}

.text-second{
    margin-top: 5px;
    margin-left: 3px;
    font-family: Roboto;
    font-size: 36px;
    font-weight: 300;
    line-height: 38px;
    letter-spacing: 0px;
}

.text-third{
    margin-top: 89px;
    margin-left: 28px;
    font-family: Roboto;
    font-size: 50px;
    font-weight: bold;
    line-height: 86px;
    letter-spacing: 1px;
    position: relative;

}

.text-third:after{
    display: block;
    content: "";
    width: 8px;
    height: 61px;
    background-color: #f0e353;
    position: absolute;
    right: 100%;
    margin-right: 15px;
    margin-top: -85px;
    

}

.text-number{
    margin-top: 26px;
    width: 162px;
    font-size: 38px;
    font-family: "Roboto";
    color: rgb(255, 255, 255);
    line-height: 1;
    font-weight: lighter;
    margin-left: 97px;
}

.number{
    text-align: center;
    font-size: 180px;
    font-family: "Roboto";
    color: rgb(255, 255, 255);
    font-weight: lighter;
}

.container {
    background-image: url('../static/back.png');
    background-size: cover;
    color: #fff;
    max-width: 100%;
    min-height: 100vh;

}
.button {
    color: rgb(240, 227, 83);
    padding: 3px 5%;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 50px;
    margin-top: 130px;
    -webkit-transition-duration: 0.4s; /* Safari */
    transition-duration: 0.4s;
    cursor: pointer;
    border: 2px solid rgb(240, 227, 83);
    background-color: transparent; 
    border-radius: 3px;
    width: 791px;
    height: 96px;
    font-weight: 500;
}

.button:hover {
    background-color: rgb(240, 227, 83);
    color: white;
    border: 2px solid white;
}

.under-button{
    font-family: "Roboto";
    font-size: 22px;
    font-weight: lighter;
    letter-spacing: -0.2px;
    margin-top: 29px;
}
</style>



