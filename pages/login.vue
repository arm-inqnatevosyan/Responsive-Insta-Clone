<!-- Arandz beqendi fronti logini ej -->
<template>
  <div>
    <Navbar />
    <form action="/action_page.php">
      <h1>Instagram</h1>
      <input type="text" placeholder="Phone number"><br>
      <input type="text" placeholder="Name and Lastname"><br>
      <input type="text" placeholder="Name User"><br>
      <input type="text" placeholder="Password">
      <p>
        Люди, которые пользуются нашим сервисом,<br> могли загрузить вашу контактную информацию в Instagram. Подробнее<br><br>
        Регистрируясь, вы принимаете наши Условия, <br>Политику конфиденциальности и Политику в <br>отношении файлов cookie.
      </p>
      <input type="submit" placeholder="Registration" class="submit">
    </form>
  </div>
</template>
<script>

</script>
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Lobster&display=swap');s
*{
    margin: 0px;
    padding: 0px;
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
    border: 1px solid rgba(128, 128, 128, 0.363);
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
@media (max-width:900px){
    form{
        width: 90%;
    }
}
      </style>
