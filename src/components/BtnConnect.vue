<template>
    <div>
        <button class="btn__connect"><img class="img__connect" src="@/assets/img/empty-wallet-add.png" alt="Изображение">Подключить кошелек</button>
    </div>
</template>

<style scoped>
@font-face {
    font-family: 'Mulish';
    src: url('@/assets/fonts/Mulish-Regular.ttf');
}

.btn__connect{
    position: relative;
    width: 287px;
    height: 39px;
    margin-right: 10px;
    padding-left: 40px;
    border: 1px solid #00C1C1;
    border-radius: 20px;
    background: none;
    color: #FFFFFF;
    font-size: 18px;
    
}
.img__connect{
    position: absolute;
    width: 24px;
    height: 24px;
    top: 6px;
    left: 30px;
    font-family: 'Mulish';
    font-weight: 700;
}
</style>