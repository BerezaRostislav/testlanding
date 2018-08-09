<template>
<v-container grid-list-xl>
<v-layout row wrap>
    <v-flex col-md-6>
        <h2 class="text-first">БЕСПЛАТНЫЙ онлайн-вебинар</h2>
        <h2 class="text-first" style="color:yellow;">ЕВРЕЙСКАЯ ЭМИГРАЦИЯ В ГЕРМАНИЮ</h2>
        <h2 class="text-second">Вопросы руководителю рускоязычного общества Германии</h2>
        <h2 class="text-first" style="margin-top:70px">25 сентября / четверг / 19-00 <span class="text-second">(киевское)</span> </h2>
    </v-flex>
    <v-flex col-md-6 style="margin-top: 70px;">
      <div style="text-align: center;">
        <span class="number">{{ this.number }} </span>
        <h3 class="text-number">мест осталось</h3>
      </div>  
    </v-flex>
</v-layout>
<v-layout align-center justify-center column >
        <button class="button" v-on:click="newnumber" >ЗАРЕГЕСТРИРОВАТСЯ</button>
        <p><i class="fa fa-code"></i>Запись предоставляется бесплатно только зарегистрированным участникам</p>

</v-layout>
</v-container>
</template>

<script>
export default {
    data() {
        return{
            number: 90,
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

h1 { 
    margin-top: 0;
    margin-bottom: 25px; 
}

h1,h2,h4
    {
        font-weight: bold;
    }

p { line-height: 1.6em;
    text-align: left;
    }

.text-first{
  font-size: 70px;
  font-family: "Roboto";
  color: rgb(255, 255, 255);
  font-weight: bold;
  line-height: 1.1;
  text-align: left;
}

.text-number{
  font-size: 30px;
  font-family: "Roboto";
  color: rgb(255, 255, 255);
  line-height: 1;
  font-weight: lighter;
}

.number{
  border: 2px solid white;
  text-align: center;
  font-size: 180px;
  font-family: "Roboto";
  color: rgb(255, 255, 255);
  line-height: 0.48;
  font-weight: lighter;
  padding: 30px;
  padding-bottom: 60px;
}

.text-second{
  font-size: 27px;
  font-family: "Roboto";
  color: rgb(255, 255, 255);
  line-height: 1.439;
  text-align: left;
  font-weight:lighter;
 
}

.text-{
  font-size: 27px;
  font-family: "Roboto";
  color: rgb(255, 255, 255);
  line-height: 1.439;
  text-align: left;
  font-weight:lighter;
 
}

@media (min-width: 992px) {
  .container {
    height: 100vh;
  }
}

@media (max-width: 991px) {
  .container {
    height: 120vh 100%;
  }
  .text-first {
      font-size: 45px;
  }
  .text-second {
      font-size: 20px;
  }
  .number {
      font-size: 140px;
  }
}

.container {
    background-image: url('../static/back.png');
    background-size: cover;
    color: #fff;
    max-width: 100%;

}
.button {
  color: rgb(240, 227, 83);
  padding: 3px 5%;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 32px;
  margin-top: 15%;
  -webkit-transition-duration: 0.4s; /* Safari */
  transition-duration: 0.4s;
  cursor: pointer;
  border: 2px solid rgb(240, 227, 83);
  background-color: transparent; 
  border-radius: 3px;

}

.button:hover {
  background-color: rgb(240, 227, 83);
  color: white;
  border: 2px solid white;
}

</style>



