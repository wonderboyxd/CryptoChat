<template>
    <div>
        <button>Посмотреть видео</button>
    </div>
</template>

<style scoped>

button{
    width: 246px;
    height: 64px;
    font-style: normal;
    font-weight: 700;
    font-size: 18px;
    color: #FFFFFF;
    border: 2px solid #00C1C1;
    border-radius: 50px;
    background: none;
    font-family: 'Mulish';
    transition: all 500ms;
}
button:hover{
    border: 2px #00C1C1 solid;
    color: white;
    transform: translateY(-8px);
}
@media (max-width: 424px) {
    button{
        
        width: 350px;
        margin-left: -5px;
        margin-bottom: 50px;
    }
}
</style>