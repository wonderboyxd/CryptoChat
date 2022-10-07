<template>
    <div class="content">
        <div class="nav-bar">
            <ul class="nav__list">
                <li class="list__item"><a class="item__link-logo" href="#">Crypto<span class="main-color">Chat</span></a></li>
                <li class="list__item"><a class="item__link" href="dsfsdf">О проекте</a></li>
                <li class="list__item"><a class="item__link" href="#">Обучение</a></li>
                <li class="list__item"><a class="item__link" href="#">FAQ</a></li>
                <li class="list__item"><a class="item__link" href="#">Контакты</a></li>
            </ul>
            <BtnConnect/>
            <BtnLogin/>
        </div>
    </div>
</template>

<script>

import BtnConnect from '@/components/BtnConnect.vue'
import BtnLogin from '@/components/BtnLogin.vue'

export default {
    components: {
        BtnConnect,
        BtnLogin
    }
}
</script>

<style scoped>
@font-face {
    font-family: 'Mulish';
    src: url('@/assets/fonts/Mulish-Regular.ttf');
}

.content{
    overflow: hidden;
    margin: 18px 0 80px 0;
    background: linear-gradient(180deg, rgba(58, 34, 127, 0.2) 0%, rgba(41, 17, 92, 0.2) 100%), #190050;
}
.nav-bar{
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    
}
.main-color{
    color: #00C1C1;
}

.nav__list{
    padding: 0;
    font-family: 'Mulish'; 
}
.list__item{
    text-align: center;
    display: inline;
    list-style: none;
    text-align: center;
    margin-right: 24px;
    font-size: 18px;
    font-weight: 700;
}

.list__item:first-child{
    margin-right: 43px;
    font-size: 22px;
    font-weight: 800;
    
}
.list__item:last-child{
    margin-right: 253px;
}

.item__link{
    text-decoration: none;
    color: rgba(255, 255, 255, 0.72);
}
.item__link-logo{
    text-decoration: none;
    color: #FFFFFF;
}
.item__link:active{
    color: #00C1C1;
}
.item__link:hover{
    color: #00C1C1;
}

@media(max-width:1439px){
    .content{
        width: 1250px;
        
    }
    .list__item{
        margin-right: 24px;
        font-weight: 700;
    }

    .list__item:first-child{
        margin-right: 43px;
        font-size: 22px;
        font-weight: 800;  
    }
    .list__item:last-child{
        margin-right: 200px;
    }

}
@media(max-width: 1023px){
     .content{
        width: 1250px;
        
    }
    .list__item{
        margin-right: 24px;
        font-size: 20px;
        font-weight: 700;
    }

    .list__item:first-child{
        margin-right: 43px;
        font-size: 22px;
        font-weight: 800;  
    }
    .list__item:last-child{
        margin-right: 200px;
    }
}
@media (max-width: 767px) {
    .content{
        width: 0;
        margin-bottom: -60px;
    }
}
@media (max-width: 424px){
    .content{
        width: 0;
        margin-bottom: -80px;
    }
}

</style>