<!--suppress CssUnknownTarget -->
<template>
  <nav>
    <div class="logo">
      <h1>Instagram</h1>
    </div>
    <div class="icons">
      <NuxtLink to="/">
        <i class="fa-solid fa-house" />
      </NuxtLink>
      <i class="fa-solid fa-magnifying-glass" />
      <NuxtLink to="/">
        <img src="./story/home.png" alt="">
      </NuxtLink>
      <img src="./story/search.png" alt="">
      <img src="./story/heart.png" alt="">
    </div>
    <ul>
      <li>
        <NuxtLink to="/">
          Home
        </NuxtLink>
      </li>
      <li>
        <NuxtLink to="/login">
          Sign In
        </NuxtLink>
      </li>
      <li>
        <NuxtLink to="/sign">
          Register
        </NuxtLink>
      </li>
    </ul>
  </nav>
</template>
<script>
export default {
  name: 'NavbarVue'
}
</script>
  <style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300&display=swap');
nav{
    width:  80%;
    height: 70px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 0 auto !important;
}
ul{
    display: flex;
    list-style: none;
    align-items: center;
}
.logo{
    font-family: 'Lobster', cursive;
    width: 200px;
}
.icons{
    width: 160px;
    display: flex;
    justify-content: space-around;
    align-items: center;
    height: 70px;
}
.icons i{
    font-size: 21px;
}
li{
    margin-left: 30px;
}
a{
    text-decoration: none;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    color: black;
}
</style>
