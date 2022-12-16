<template>
  <div class="post">
    <main>
      <div class="post-div">
        <img src="./insta6.jpg" alt="">
        <div class="global">
          <p>robincield</p>
          <div class="icons">
            <p>300<img src="../story/heart.png" alt=""></p>
            <img src="../story/comment.png" alt="">
            <img src="../story/send.png" alt="">
          </div>
        </div>
        <div class="p">
          <p>armenia</p>
          <p>paris</p>
          <p>russia</p>
          <p>armenia</p>
          <p>paris</p>
          <p>russia</p>
          <p>armenia</p>
          <p>paris</p>
          <p>russia</p>
        </div>
      </div>
      <div class="post-div">
        <img src="./insta7.jpg" alt="">
        <div class="global">
          <p>arnauld</p>
          <div class="icons">
            <p>100<img src="../story/heart.png" alt=""></p>
            <img src="../story/comment.png" alt="">
            <img src="../story/send.png" alt="">
          </div>
        </div>
        <div class="p">
          <p>armenia</p>
          <p>paris</p>
          <p>russia</p>
        </div>
      </div>

      <div class="post-div">
        <img src="./insta5.jpg" alt="">
        <div class="global">
          <p>tinanakey</p>
          <div class="icons">
            <p>400<img src="../story/heart.png" alt=""></p>
            <img src="../story/comment.png" alt="">
            <img src="../story/send.png" alt="">
          </div>
        </div>
        <div class="p">
          <p>armenia</p>
          <p>paris</p>
          <p>russia</p>
          <p>armenia</p>
          <p>paris</p>
          <p>russia</p>
          <p>armenia</p>
          <p>paris</p>
          <p>russia</p>
        </div>
      </div>
      <div class="post-div">
        <img src="./insta4.webp" alt="">
        <div class="global">
          <p>louwsers</p>
          <div class="icons">
            <p>500<img src="../story/heart.png" alt=""></p>
            <img src="../story/comment.png" alt="">
            <img src="../story/send.png" alt="">
          </div>
        </div>
        <div class="p3" />
      </div>
    </main>
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
export default {
  name: 'PostsVue'
}
</script>
<style>
.post{
    margin-top: 30px;
    width: 100%;
}
main{
    width: 95%;
    display: grid;
    grid-template-columns: repeat(2,1fr);
  margin: 30px auto 0;
}
main .post-div{
    width:70%;
    margin: 0 auto;
}
main img{
    height: 400px;
    width:100%;
    overflow: hidden;
}
.global{
    display: flex !important;
    justify-content: space-between !important;
    width: 98%;
    height: 40px;
    margin-top: 10px;
    font-family:Verdana, Geneva, Tahoma, sans-serif;
}
.icons{
    display: flex;
}
.icons p{
    font-size: 13px;
    margin-left: 10px;
}
.global p{
    margin-left: 10px;
}
.p{
    margin-left: 10px;
    font-family: Arial, Helvetica, sans-serif;
    line-height: 24px;
}
.icons img{
    width: 20px;
    height: 20px;
    margin-left: 10px;
}
footer{
    width: 100%;
    display: flex;
    margin-top: 50px;
}
footer ul{
    width: 80%;
    height: 50px;
    display: flex;
    margin: 0 auto;
    justify-content: space-around;
    align-items: center;
    list-style: none;
}
footer ul li{
    text-decoration: none;
    font-family: sans-serif;
    color: rgb(0, 0, 0) !important;
    font-size: 13px;
}
@media (max-width:800px){
    main{
        grid-template-columns: repeat(1,1fr);
    }
  footer{
    margin-top: 200px;
  }
  footer ul{
    display: flex;
    flex-direction: column;
  }
  footer ul li {
    margin-top: 20px;
    border-bottom:2px solid rgba(0, 0, 0, 0.51);
  }
}
@media (max-width: 500px){
  footer{
    display: none;
  }
  main .post-div{
    width: 100%;
  }
}
</style>
