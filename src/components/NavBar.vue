<template>
    <div class="content">
        <div class="nav-bar">
            <ul class="nav__list">
                <li class="list__item logo"><a class="item__link" href="#">Crypto<span class="main-color">Chat</span></a></li>
                <li class="list__item"><a class="item__link" href="#">О проекте</a></li>
                <li class="list__item"><a class="item__link" href="#">Обучение</a></li>
                <li class="list__item"><a class="item__link" href="#">FAQ</a></li>
                <li class="list__item"><a class="item__link" href="#">Контакты</a></li>
            </ul>
            <BtnConnect/>
            <BtnLogon/>
        </div>
    </div>
</template>

<script>

import BtnConnect from '@/components/BtnConnect.vue'
import BtnLogon from '@/components/BtnLogon.vue'

export default {
    components: {
        BtnConnect,
        BtnLogon
    }
}
</script>

<style>

.content{
    align-items: center;
}
.nav-bar{
    display: flex;
    align-items: center;
    justify-content: center;
}
.main-color{
    color: blue;
}
.nav__list{
    padding: 0;
    margin-top: 18px;
    margin-bottom: 0px;
   
}
.list__item{
    display: inline;
    list-style: none;
    text-align: center;
    margin-right: 24px;
}
.list__item:first-child{
    margin-right: 43px;
}
.list__item:last-child{
    margin-right: 253px;
}
.item__link{
    text-decoration: none;
}
</style>