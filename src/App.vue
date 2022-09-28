<template>
  <div class="container">
    <NavBar />
    <div class="main__section">
      <div class="section__left-wrapper">
        <h1>Единое <span class="main-color">место общения</span> вашего сообщества</h1>
        <p>Первое децентрализованное решение<br> на мировом рынке</p>
        <div class="section__left-wrapper-buttons">
          <BtnOpenchat/>
          <BtnWatchvideo/>
        </div>
      </div>
      <div class="section__right-wrapper">
        <img src="@/assets/img/Illustration.png" alt="Изображение">
    </div>
    </div>
    <div class="section__private">
      <div class="private__title">
        <h2>Приватность на 100%</h2>
        </div>
      <div class="private__info-block">
        <div class="info-block">
          <img src="@/assets/img/eye.png" alt="Изображение">
          <h3>Приватность</h3>
          <p>Сообщения открыты всем<br>или зашифрованы от других<br> пользователей на ваш выбор</p>
        </div>
        <div class="info-block">
          <img src="@/assets/img/document.png" alt="Изображение">
          <h3>Хранение</h3>
          <p>Каждое сообщение хранится<br>в Smart-контракте</p>
        </div>
        <div class="info-block">
          <img src="@/assets/img/connection.png" alt="">
          <h3>DEX-решение</h3>
          <p>Площадка выдерживает<br>многомиллионную аудиторию за<br>счет отсутствия какой-либо<br>серверной части</p>
        </div>
      </div>
    </div>
    
  </div>
</template>

<script>

import NavBar from '@/components/NavBar.vue'
import BtnOpenchat from '@/components/BtnChatopen.vue'
import BtnWatchvideo from '@/components/BtnWatchvideo.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    BtnOpenchat,
    BtnWatchvideo
    
  }
}
</script>

<style>
@font-face {
    font-family: 'Mulish';
    src: url('@/assets/fonts/Mulish-Regular.ttf');
}

body{
  margin: 0;
  background: #1A0050;
  box-sizing: border-box;
}
.container{
  margin: 0;
  width: 100%;
  height: 100%;
  align-items: center;
}
.main__section{
  display: flex;
  align-items: center;
  justify-content: center;
  align-items: center;
  color: #FFFFFF;
  margin: 0 0 100px 60px;
}
.main-color{
    color: #00C1C1;
}
.section__left-wrapper{
  width: 770px;
  height: 340px;
  align-items: center;
  font-family: 'Mulish';
  font-style: normal;
  font-weight: 700;
  font-size: 30px;  
}
.section__left-wrapper h1{
  margin: 0 0 32px 0;
}
.section__left-wrapper p {
  margin: 0 0 52px 0;
  text-decoration: none;
  color: rgba(255, 255, 255, 0.72);
}
.section__left-wrapper-buttons{
  display: inline-flex;
}
.section__rigth-wrapper{
  align-items: center;
}

.section__private{
  margin: 0;
  color: #FFFFFF;
}
.private__title{
  font-size: 32px;
  text-align: center;
  margin-bottom: 48px;
}
.private__info-block{
  display: flex;
  justify-content: center ;
  align-items: center;
}
.info-block{
  
}
.info-block h3{
  font-size: 24px;
}
.info-block p{
  text-decoration: none;
  color:rgba(255, 255, 255, 0.72); ;
  font-size: 18px;
}


</style>
