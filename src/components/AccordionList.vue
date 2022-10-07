<template>
    <div class="container">
        <div class="accordion__list">
            <div @click="open" class="accordion">Вопрос 1</div>
            <div class="panel">
                <p v-if="show == false ">Ответ на вопрос в «аккардеоне»</p>
            </div>
            <div @click="open" class="accordion">Вопрос 2</div>
            <div class="panel">
                <p v-if="show == false">Ответ на вопрос в «аккардеоне»</p>
            </div>
            <div @click="open" class="accordion">Вопрос 3</div>
            <div class="panel">
                <p v-if="show == false">Ответ на вопрос в «аккардеоне»</p>
            </div>
            <div @click="open" class="accordion">Вопрос 4</div>
            <div class="panel">
                <p v-if="show == false">Ответ на вопрос в «аккардеоне»</p>
            </div>
        </div>
    </div>
</template>
<script>
export default {
   data() {
    return {
        show: true
    }
   },
   methods: {
    open: function(event){
        this.show = !this.show
        var matches = document.querySelectorAll('.accordion');
          for(var i = 0; i < matches.length; i++) {
              matches[i].classList.remove('active');
           }
        event.target.classList.toggle('active');
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
    content: url(@/assets/img/arrowDown.png);
    display: block;

}
.accordion.active::after{
    content: url(@/assets/img/arrowUp.png);
    
}
.accordion:hover{
    background-color:rgba(109, 40, 222, 0.4);
}

.panel{
    display: none;
    padding: 0 18px;
    background-color: rgba(109, 40, 222, 0.4);
    color: #FFFFFF;
    overflow: hidden;
    
}

.accordion.active + .panel {
    display: block ;
    
}
@media (max-width: 1439px) {
     .container{
        width: 100%;
        margin-left: 80px;
    }
}
@media (max-width: 1023px) {
    .container{
        width: 100%;
        margin-left: 0px;
    }
}

@media (max-width: 424px){
    .accordion__list{
        width: 350px;
        margin-left: 13px;
    }
    .accordion{
        font-size: 16px;
    }
    .panel{
        font-size: 14px;
    }
}
</style>