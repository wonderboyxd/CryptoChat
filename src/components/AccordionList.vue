<template>
    <div class="accordion__list">
        <button @click="show = !show" class="accordion">Вопрос 1</button>
        <div class="panel">
            <p v-if="show">Ответ на вопрос в «аккардеоне»</p>
        </div>
        <button class="accordion">Вопрос 2</button>
        <div class="panel">
            <p>Ответ на вопрос в «аккардеоне»</p>
        </div>
        <button class="accordion">Вопрос 3</button>
        <div class="panel">
            <p>Ответ на вопрос в «аккардеоне»</p>
        </div>
        <button class="accordion">Вопрос 4</button>
        <div class="panel">
            <p>Ответ на вопрос в «аккардеоне»</p>
        </div>
    </div>
</template>
<script>
export default {
   data() {
    return {
        show: false
    }
   }
}
</script>


<style scoped>
.accordion__list{
    width: 700px;
    margin-left: calc((100% - 700px) / 2);
    margin-bottom: 96px;
}
.accordion{
    width: 100%;
    padding: 30px;
    display: flex;
    justify-content: space-between;
    text-align: left;
    background: none;

    border: none;
    border-bottom: 1px #00C1C1 solid;
    outline: none;
    transition: 0.4s;

    font-family: 'Mulish';
    font-style: normal;
    font-weight: 700;
    font-size: 18px;
    line-height: 24px;
    color: #FFFFFF;
}
.accordion::after{
    content: url(@/assets/img/arrow.png);

}
.active, .accordion:hover{
    background-color:rgba(109, 40, 222, 0.4);
}
.panel {
  padding: 0 18px;
  background-color: white;
  display: none;
  overflow: hidden;
}

</style>