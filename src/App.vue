<template>
  <div class="container">
    <NavBar />
    <div class="main__section">
      <div class="section__left-wrapper">
        <h1>Единое <span class="main-color">место общения </span>вашего сообщества</h1>
        <p>Первое децентрализованное решение на мировом рынке</p>
        <div class="section__left-wrapper-buttons">
          <BtnOpenchat/>
          <BtnWatchvideo/>
        </div>
      </div>
      <div class="section__right-wrapper">
        <img class="right-wrapper__img" src="@/assets/img/Illustration.png" alt="Изображение">
      </div>
    </div>

    <div class="section__private">
      <div class="private__title">
        <h2>Приватность на 100%</h2>
        </div>
      <div class="private__info-block">
        <div class="info-block">
          <div class="info-block__img">
            <img class="block-img" src="@/assets/img/eye.png" alt="Изображение">
          </div>
          <div class="info-block__text">
            <h3>Приватность</h3>
            <p>Сообщения открыты всем<br>или зашифрованы от других<br> пользователей на ваш выбор</p>
          </div>
        </div>

        <div class="info-block">
          <div class="info-block__img">
            <img class="block-img" src="@/assets/img/document.png" alt="Изображение">
          </div>
          <div class="info-block__text">
            <h3>Хранение</h3>
          <p>Каждое сообщение хранится<br>в Smart-контракте</p>
          </div>
        </div>

        <div class="info-block">
          <div  class="info-block__img">
            <img class="block-img" src="@/assets/img/connection.png" alt="">
          </div>
          <div class="info-block__text">
            <h3>DEX-решение</h3>
          <p>Площадка выдерживает<br>многомиллионную аудиторию<br>за счет отсутствия какой-либо<br>серверной части</p>
          </div>
        </div>
      </div>
    </div>
    <div class="section__video">
      <div class="video__img">
        <iframe width="650" height="350" src="https://www.youtube.com/embed/i5kUQl6hvoo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </div>
      <div class="video__text">
        <h3>Посмотри обучающее<br>видео</h3>
        <ul class="video__text-list">
          <li class="text-list__item">Этап 1. Тут расписан первый этап</li>
          <li class="text-list__item">Этап 2. Тут расписан первый этап</li>
          <li class="text-list__item">Этап 3. Тут расписан первый этап</li>
          <li class="text-list__item">Этап 4. Тут расписан первый этап</li>
          <li class="text-list__item">Этап 5. Тут расписан первый этап</li>
        </ul>
      </div>
    </div>
    <div class="section__mechanics">
      
        <div class="mechanics__left-wrapper">
          <h2>Игровая механика покупки и продажи смайликов, аватаров<br>и прочих NFT-объектов в чате</h2>
          <p>Какой-то уточняющий текст про покупку и продажу<br>смайликов/аваторов и прочего-прочего</p>
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
        <img class="left-wrapper__img" src="@/assets/img/FrameSelary.png" alt="Изображение">
      </div>
      <div class="selary__rigth_wrapper">
        <h2>Ваш заработок на сборе комиссий с сообщений<br>пользователей!</h2>
        <p>Какой-то уточняющий текст про заработок от крипточата.</p>
        <div class="rigth_wrapper__text">
          <h4>300 M+</h4>
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
        <h2>Готовы вывести своё сообщество на новый уровень? Начните с <span class="main-color">CryptoChat</span></h2>
        <BtnConnectcryptochat/>
      </div>
    </div>
    <FooterBlock/>
  </div>
</template>

<script>

import NavBar from '@/components/NavBar.vue'
import BtnOpenchat from '@/components/BtnChatopen.vue'
import BtnJoinchat from '@/components/BtnChatjoin.vue'
import AccordionList from '@/components/AccordionList.vue'
import BtnConnectcryptochat from '@/components/BtnConnectcryptochat.vue'
import FooterBlock from '@/components/FooterBlock.vue'
import BtnWatchvideo from '@/components/BtnWatchvideo.vue'

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

<style src="./app.css">

</style>
