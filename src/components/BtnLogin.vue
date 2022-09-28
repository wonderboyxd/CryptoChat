<template>
    <div >
        <button class="btn__login"><img class="img__login" src="@/assets/img/login.png" alt="Изображение">Войти в чат</button>
    </div>
</template>

<script>

</script>
<style scoped>
@font-face {
    font-family: 'Mulish';
    src: url('@/assets/fonts/Mulish-Regular.ttf');
}

.btn__login{
    position: relative;
    width: 192px;
    height: 40px;
    padding-left: 30px;
    font-size: 18px;
    color: #FFFFFF;
    background: #00C1C1;
    border-radius: 20px;
    
}
.img__login{
    position: absolute;
    width: 24px;
    height: 24px;
    top: 6px;
    left: 22px;
    font-family: 'Mulish';
    font-weight: 700;
}
</style>