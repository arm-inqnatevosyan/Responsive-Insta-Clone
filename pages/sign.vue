<!-- Arandz beqendi fronti registri ej -->
<template>
  <div>
    <Navbar />
    <div class="block">
      <form @submit.prevent="submit">
        <h1>Instagram</h1>
        <p class="one">
          Зарегистрируйтесь, чтобы смотреть фото и видео ваших друзей.
        </p>
        <button>Open your Facebook</button>
        <div class="inputs">
          <input v-model="data.name" type="text" placeholder="Name User">
          <input v-model="data.email" type="email" placeholder="Email">
          <input v-model="data.password" type="password" placeholder="Password">
        </div>
        <p>Люди, которые пользуются нашим сервисом,<br> могли загрузить вашу контактную информацию <br>в Instagram. Подробнее</p>
        <p>Регистрируясь, вы принимаете наши Условия,<br> Политику конфиденциальности и Политику в <br>отношении файлов cookie.</p>
        <button class="reg">
          Registracia
        </button>
      </form>
    </div>
    <footer>
      <ul>
        <li>Meta</li>
        <li>Информация</li>
        <li>Блог</li>
        <li>Вакансии</li>
        <li>API</li>
        <li>Конфиденциальность</li>
        <li>Условия</li>
        <li>Популярные аккаунты</li>
        <li>Хэштеги</li>
        <li>Места</li>
        <li>Instagram Lite</li>
      </ul>
    </footer>
  </div>
</template>
<script>
import { reactive } from 'vue'

export default {
  name: 'Register',
  setup () {
    const data = reactive({
      name: '',
      email: '',
      password: ''
    })

    const submit = async () => {
      await fetch('http://localhost:8000/api/register', {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify(data)
      })
    }
    return {
      data,
      submit
    }
  }
}
</script>
<style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Lobster&display=swap');

    .block{
        height: 78vh;
        width: 40%;
        border: 1px solid rgba(128, 128, 128, 0.363);
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;
        padding: 20px;
        margin: 20px auto;
        }
        .block h1{
            font-family: 'Lobster', cursive;
            font-weight: 400;
            font-size: 30px;
            height: 60px;
        }
        .one{
            color: grey;
            font-size: 15px !important;
        }
        .block p{
            font-family:Verdana, Geneva, Tahoma, sans-serif;
            font-size: 13px;
            text-align: center;
            line-height: 30px;
            color: rgb(63, 61, 61);
        }
        .block button{
            width: 250px;
            height: 30px;
            outline: none;
            border: none;
            background-color: rgb(40, 166, 224);
            color: white;
           font-family: sans-serif;
           border-radius: 5px;
           margin-top: 30px;
        }
        .block div{
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        .inputs{
            display: flex;
            flex-direction: column;
        }

        .inputs{
            margin-top: 10px;
        }
        .inputs input{
            margin-top: 20px;
            width: 380px;
            height: 40px;
            outline: none;
            border: none;
            border: 1px solid rgba(128, 128, 128, 0.363);
            font-family: Verdana, Geneva, Tahoma, sans-serif;
            padding-left: 10px;
            border-radius: 5px;
            background-color: rgba(211, 201, 201, 0.192);
        }
        ::-webkit-input-placeholder{
            color: grey;
        }
        .reg{
            width: 150px;
            height: 30px;
            outline: none;
            border: none;
            background-color: rgb(40, 166, 224);
            color: white;
           font-family: sans-serif;
           border-radius: 5px;
        }
        @media (max-width:900px){
            img{
                display: none;
            }
            main{
                display: flex;
                justify-content: center;
                align-items: center;
                width: 100%;
            }
            .block{
                width: 85%;
            }
        }
        footer{
            width: 100%;
            display: flex;
        }
        footer ul{
            width: 100%;
            display: flex;
            justify-content: space-around;
            list-style: none;
        }
        footer ul li{
            text-decoration: none;
            font-family: sans-serif;
            color: grey !important;
            font-size: 13px;
        }
    </style>
