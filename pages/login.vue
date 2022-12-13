<!--Arandz beqendi fronti loginiej -->
<template>
  <div>
    <Navbar />
    <form>
      <h1>Instagram</h1>
      <input type="text" placeholder="Phone number"><br>
      <input type="text" placeholder="Name and Lastname"><br>
      <input type="text" placeholder="Name User"><br>
      <input type="text" placeholder="Password">
      <p>
        Люди, которые пользуются нашим сервисом,
      </p><p> могли загрузить вашу контактную информацию в Instagram. Подробнее</p>
      <p>Регистрируясь, вы принимаете наши Условия,</p> <p>Политику конфиденциальности и Политику в</p> <p>отношении файлов cookie.</p>
      <input type="submit" placeholder="Registration" class="submit">
    </form>
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
import Navbar from '~/components/Navbar.vue'

export default {
  components: { Navbar }
}
</script>
<!--suppress CssUnknownTarget -->
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Lobster&display=swap');
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
form{
    width: 40%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin: 20px auto;
    text-align: left;
    height: 80vh;
    border: 1px solid rgba(128, 128, 128, 0.363);
    color: black;
}
form h1{
    font-family: 'Lobster', cursive;
    font-weight: 400;
    font-size: 40px;
    color: black;
    margin-bottom: 20px;
}
form input{
    width: 380px;
    height: 40px;
    outline: none;
    border: none;
    color:rgb(65, 62, 62) !important;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    padding-left: 10px;
  border-radius: 5px;
}
::-webkit-input-placeholder{
    color: grey;
}
.submit{
    color: white !important;
    background-color: rgb(40, 166, 224);
    margin-top: 50px;
}
form p{
    width: 380px;
    text-align: center;
    margin-top: 20px;
    line-height: 23px;
    font-size: 13px;
    color: rgb(63, 61, 61);
    font-family: Verdana, Geneva, Tahoma, sans-serif;
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
  font-family:  sans-serif;
  color: grey !important;
  font-size: 13px;
}
@media (max-width:900px){
    form{
        width: 90%;
    }
  footer{
    margin-top: 250px;
  }
  footer ul li {
    margin-top: 30px;
  }
}
      </style>
