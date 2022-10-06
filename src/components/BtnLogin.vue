<template>
    <div >
        <button><img src="@/assets/img/login.png" alt="Изображение">Войти в чат</button>
    </div>
</template>

<script>

</script>
<style scoped>
@font-face {
    font-family: 'Mulish';
    src: url('@/assets/fonts/Mulish-Regular.ttf');
}

button{
    position: relative;
    width: 192px;
    height: 40px;
    padding-left: 30px;
    font-size: 18px;
    color: #FFFFFF;
    background: #00C1C1;
    border-radius: 20px;
    transition: all 500ms;
}

button:hover{
    border: 2px #00C1C1 solid;
    transform: translateY(-8px);
}

img{
    position: absolute;
    width: 24px;
    height: 24px;
    top: 6px;
    left: 22px;
    font-family: 'Mulish';
    font-weight: 700;
}
@media (max-width:1439px) {
    button{
    
    width: 160px;
    height: 39px;
    margin-right: 10px;
    padding-left: 30px;
    font-size: 18px;
    
    }
    img{
        position: absolute;
        width: 22px;
        height: 22px;
        top: 6px;
        left: 12px;
        font-family: 'Mulish';
        font-weight: 700;
    }
}
@media (max-width:1023px) {
    button{
    width: 150px;
    height: 39px;
    margin-right: 10px;
    padding-left: 25px;
    font-size: 18px;
    }
    img{
        position: absolute;
        width: 20px;
        height: 20px;
        top: 6px;
        left: 8px;
        font-family: 'Mulish';
        font-weight: 700;
    }
}
</style>