<template>
  <div class="container">
    <NavBar />
    <div class="main__section">
      <div class="section__left-wrapper">
        <h1>Единое <span class="main-color">место общения</span><br>вашего сообщества</h1>
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
          <div class="info-block__img">
            <img src="@/assets/img/eye.png" alt="Изображение">
          </div>
          <div class="info-block__text">
            <h3>Приватность</h3>
            <p>Сообщения открыты всем<br>или зашифрованы от других<br> пользователей на ваш выбор</p>
          </div>
        </div>

        <div class="info-block">
          <div class="info-block__img">
            <img src="@/assets/img/document.png" alt="Изображение">
          </div>
          <div class="info-block__text">
            <h3>Хранение</h3>
          <p>Каждое сообщение хранится<br>в Smart-контракте</p>
          </div>
        </div>

        <div class="info-block">
          <div class="info-block__img">
            <img src="@/assets/img/connection.png" alt="">
          </div>
          <div class="info-block__text">
            <h3>DEX-решение</h3>
          <p>Площадка выдерживает<br>многомиллионную аудиторию за<br>счет отсутствия какой-либо<br>серверной части</p>
          </div>
        </div>
      </div>
    </div>
    <div class="section__video">
      <div class="video__img">
        <img class="video__image" src="@/assets/img/Rectangle1.png" alt="Изображение">
        <img class="video__play" src="@/assets/img/FramePlay.png" alt="">
      </div>
      <div class="video__text">
        <h3>Посмотри обучающее<br>видео</h3>
        <ul class="video__text-list">
          <ol class="text-list__item">Этап 1. Тут расписан первый этап</ol>
          <ol class="text-list__item">Этап 2. Тут расписан первый этап</ol>
          <ol class="text-list__item">Этап 3. Тут расписан первый этап</ol>
          <ol class="text-list__item">Этап 4. Тут расписан первый этап</ol>
          <ol class="text-list__item">Этап 5. Тут расписан первый этап</ol>
        </ul>
      </div>
    </div>
    <div class="section__mechanics">
      
        <div class="mechanics__left-wrapper">
          <h1>Игровая механика покупки и<br> продажи смайликов, аватаров<br>и прочих NFT-объектов в чате</h1>
          <p>Какой-то уточняющий текст про покупку и продажу<br>сайликов/аваторов и прочего-прочего</p>
          <div class="mechanics__left-wrapper-button">
            <BtnJoinchat />
          </div>
        </div>
        <div class="mechanics__right_wrapper">
          <img class="mechanics__img" src="@/assets/img/Illustrations2.png" alt="Изображение">
        </div>
      
    </div>
    <div class="section__selary">
      <div class="selary__left_wrapper">
        <img src="@/assets/img/FrameSelary.png" alt="Изображение">
      </div>
      <div class="selary__rigth_wrapper">
        <h2>Ваш заработок на сборе<br>комиссий с сообщений<br>пользователей!</h2>
        <p>Какой-то уточняющий текст про заработок<br>от крипточата.</p>
        <div class="rigth_wrapper__text">
          <h3>300 M+</h3>
          <p>Пользователей Blockchain-<br>технолгии на 2022г</p>
        </div>
      </div>
    </div>
    <div class="questions__title">
      <h2>Остались вопросы?</h2>
    </div>
    <AccordionList/>

    <div class="section__last_block">
      <div class="last_block__text">
        <h2>Готовы вывести своё<br>сообщество на новый уровень?<br>Начните с <span class="main-color">CryptoChat</span></h2>
        <BtnConnectcryptochat/>
      </div>
    </div>
    <FooterBlock/>
  </div>
</template>

<script>

import NavBar from '@/components/NavBar.vue'
import BtnOpenchat from '@/components/BtnChatopen.vue'
import BtnWatchvideo from '@/components/BtnWatchvideo.vue'
import BtnJoinchat from '@/components/BtnChatjoin.vue'
import AccordionList from '@/components/AccordionList.vue'
import BtnConnectcryptochat from '@/components/BtnConnectcryptochat.vue'
import FooterBlock from '@/components/FooterBlock.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    BtnOpenchat,
    BtnWatchvideo,
    BtnJoinchat,
    AccordionList,
    BtnConnectcryptochat,
    FooterBlock
    
  }
}
</script>

<style>
@font-face {
    font-family: 'Mulish';
    font-family: 'DM Sans';
    src: url('@/assets/fonts/Mulish-Regular.ttf');
    src: url('@/assets/fonts/DMSans-Regular.ttf')
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
  justify-content: center;
  align-items: center;
  color: #FFFFFF;
  margin: 0 0 110px 60px;
}
.main-color{
    color: #00C1C1;
}
.section__left-wrapper{
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


.section__private{
  margin: 0 0 48px 0;
  color: #FFFFFF;
}
.private__title{
  font-family: 'Mulish';
  font-style: normal;
  font-weight: 700;
  font-size: 32px;
  text-align: center;
  margin-bottom: 48px;
}
.private__info-block{
  display: flex;
  justify-content: center ;
  align-items: center;
  margin-right: 48px;
}
.private__info-block:last-child{
  margin-right: 0px;
}
.info-block{
  display: flex;
  width: 400px;
  height: 200px;
  flex-wrap: wrap;
}
.info-block__img{
  margin-right: 23px;
}
.info-block h3{
  font-size: 24px;
  margin: 0 0 13px 0;
}
.info-block p{
  text-decoration: none;
  color:rgba(255, 255, 255, 0.72); ;
  font-size: 18px;
}

.section__video{
  width: 1288px;
  height: 442px;
  display: flex;
  justify-content: center;
  background: #FFFFFF;
  border-radius: 20px;
  margin-left: calc((100% - 1288px)/2);
  margin-bottom: 72px;
}
.video__img{
  margin: 46px 76px 0 0;
  position: relative;
}
.video__play{
  z-index: 1;
  position: absolute;
  top: 30%;
  left: 43%;
}
.video__text{
  text-align: left;
}
.video__text h3{
  font-family: 'Mulish';
  font-style: normal;
  font-weight: 700;
  font-size: 40px;
  line-height: 40px;
  color: #1A0050;
  margin-bottom: 48px;
}
.video__text-list{
  padding: 0;
  margin: 0;
  font-family: 'Mulish';
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  line-height: 24px;
  color: rgba(8, 8, 8, 0.56);
}
.text-list__item{
  margin-bottom: 17px;
  padding: 0;
}

.section__mechanics{
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 105px;
  color: #FFFFFF;
  background-color:rgba(109, 40, 222, 0.4);
}

.mechanics__left-wrapper{
  align-items: center;
  font-family: 'Mulish';
  font-style: normal;
  font-weight: 700;
  font-size: 18px;  
  margin-left: 40px;
}
.mechanics__left-wrapper h1{
  margin: 0 0 32px 0;
}
.mechanics__left-wrapper p {
  margin: 0 0 52px 0;
  text-decoration: none;
  color: rgba(255, 255, 255, 0.72);
}
.mechanics__left-wrapper-buttons{
  display: inline-flex;
}
.mechanics__rigth-wrapper{
  padding-top: 50px ;
  align-items: center;
}
.mechanics__right_wrapper{
  margin-top: 88px;
}


.section__selary{
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 114px;
}
.selary__left_wrapper{
  margin-right: 151px;
}
.selary__rigth_wrapper h2{
  margin: 0 0 22px 0;
  font-family: 'Mulish';
  font-style: normal;
  font-weight: 700;
  font-size: 40px;
  line-height: 40px;

  color: #FFFFFF;
}
.selary__rigth_wrapper p {
  margin: 0 0 67px 0;
  font-family: 'Mulish';
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  line-height: 24px;
  color: rgba(255, 255, 255, 0.72);
}
.rigth_wrapper__text{
  display: flex;
}
.rigth_wrapper__text h3{
  margin: 0 16px 0 0;
  padding: 0;
  font-family: 'DM Sans';
  font-style: normal;
  font-weight: 500;
  font-size: 42px;
  color: #00C1C1;
}
.rigth_wrapper__text p{
  margin: 0;
  padding: 0;
  font-family: 'DM Sans';
  font-style: normal;
  font-weight: 400;
  font-size: 16px; 
}


.questions__title{
  display: flex;
  justify-content: center;
  font-family: 'Mulish';
  font-style: normal;
  font-weight: 700;
  font-size: 40px;
  line-height: 32px;
  color: #FFFFFF;
  margin-bottom: 48px;
}

.section__last_block{
  display: flex;
  justify-content: center;
  width: 1192px;
  height: 456px;
  background: #6D28DE;
  border-radius: 20px;
  margin-left: calc((100% - 1192px) / 2);
  margin-bottom: 155px;
  text-align: center;
  color: #FFFFFF;
}
.last_block__text{
  font-family: 'Mulish';
  font-style: normal;
  font-weight: 700;
  font-size: 40px;
}
.last_block__text h2{
  margin-bottom: 64px;
}


</style>
