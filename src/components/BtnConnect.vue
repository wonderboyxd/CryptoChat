<template>
    <div>
        <button><img src="@/assets/img/empty-wallet-add.png" alt="Изображение">Подключить кошелек</button>
    </div>
</template>

<style scoped>
@font-face {
    font-family: 'Mulish';
    src: url('@/assets/fonts/Mulish-Regular.ttf');
}

button{
    position: relative;
    width: 287px;
    height: 39px;
    margin-right: 10px;
    padding-left: 40px;
    border: 2px solid #00C1C1;
    border-radius: 20px;
    background: none;
    color: #FFFFFF;
    font-size: 18px;
    transition: all 300ms;
}
button:hover{
    transform: translateY(-8px);
}
img{
    position: absolute;
    width: 24px;
    height: 24px;
    top: 6px;
    left: 30px;
    font-family: 'Mulish';
    font-weight: 700;
}
</style>