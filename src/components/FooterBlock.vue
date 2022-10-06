<template>
    <div class="footer_container">
        <div class="footer__nav">
            <div class="elements">
                <div class="name">Crypto<span class="colored">Chat</span></div>
                <div class="social__icons">
                    <img class="img" src="@/assets/img/Twitter.png" alt="Иконка">
                    <img class="img" src="@/assets/img/Facebook.png" alt="Иконка">
                    <img class="img" src="@/assets/img/Inst.png" alt="Иконка">
                    <img class="img" src="@/assets/img/Github.png" alt="Иконка">
                </div>
            </div>  
            
        </div>
        <hr>
        <div class="confidence">
            <div class="confidence__items">
                <p>© Copyright 2022, All Rights Reserved</p>
                <div class="confidence__right_text">
                    <p>Privacy Policy</p>
                    <p>Terms & Conditions</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.footer_container{
    width: 1190px;
    height: 59px;
    margin-left: calc((100% - 1190px) / 2);
}
.elements{
    display: flex;
    justify-content: space-between;
}
.name{
    color: #FFFFFF;
    margin-bottom: 36px;
    font-family: 'Mulish';
    font-style: normal;
    font-weight: 800;
    font-size: 22px;
    line-height: 28px;
}
.colored{
    color:  #00C1C1;
}
.img{
    vertical-align: middle;
    margin: auto 0;
    margin-right: 37px;
}
.img:last-child{
    margin-right: 0;
}
.social__icons{
    margin-bottom: 36px;
}
.confidence{
    color: #797B89;
    
}
.confidence__items{
    display: flex;
    justify-content: space-between;
}
.confidence__right_text{
    display: flex;
    font-family: 'DM Sans';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
}
.confidence__right_text p{
    margin-right: 50px;
}
.confidence__right_text p:last-child{
    margin-right: 0;
}

@media (max-width: 1199px){
    .footer_container{
        width: 960px;
        margin-left: 150px;
    }
}
@media (max-width: 991px){
    .footer_container{
        width: 720px;
        margin-left: 250px;
    }
}
@media (max-width: 767px){
    .footer_container{
        width: 540px;
        margin-left: 350px;
    }
}
@media (max-width: 575px){
    .footer_container{
        width: 100%;
        margin-left: 400px;
    }
}
</style>