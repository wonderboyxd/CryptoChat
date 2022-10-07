<template>
    <div>
        <button>Войти в чат</button>
    </div>
</template>

<style scoped>
button{
    width: 186px;
    height: 64px;
    margin: 0;
    padding: 0;
    background: #00C1C1;
    border-radius: 16px;
    font-family: 'Mulish';
    font-style: normal;
    font-weight: 700;
    font-size: 18px;
    color: #FFFFFF;
    transition: all 500ms;
}

button:hover{
    border: 2px #00C1C1 solid;
    transform: translateY(-8px);
}

@media (max-width: 424px) {
    button{
        width: 340px;
        border-radius: 50px;
        margin-bottom: -20px;
        
    }
}
</style>