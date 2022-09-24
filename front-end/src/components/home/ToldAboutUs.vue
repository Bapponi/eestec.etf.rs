
<template>
<!-- // ova stranica treba bolje da se optimizuje sto se tice vue-a -->
    <div class="toldAboutUs">
        <img src="../../assets/ilustrations/hramR.png" alt="sasChurch" id="sasChurch">
        <h1 id="aboutUsTitle">Rekli su o nama</h1>
        <div class="commentPanels">
            <div class="commentPanel">
                <div class="imgComm">
                    <div class="imgPart">
                        <img src="../../assets/Bubalo.jpg" alt="Bubi gang" class="inImgPart">
                    </div>
                    <div class="arrowLeft"></div>
                </div>
                
                <div class="textPart">
                    <Comment text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Turpis euismod porta laoreet molestie id sed bibendum. Blandit facilisi bibendum et, ullamcorper ac. 
                    Habitasse elit tellus vitae nulla quisque blandit fermentum. Volutpat aenean volutpat diam vel, facilisi. Quam porttitor sed pellentesque in elementum lacus tellus. Mauris 
                    sed tellus quis mattis egestas viverra. Morbi netus in pellentesque laoreet duis massa.
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Turpis euismod porta laoreet molestie id sed bibendum. Blandit facilisi bibendum et, ullamcorper ac. 
                    Habitasse elit tellus vitae nulla quisque blandit fermentum. Volutpat aenean volutpat diam vel," who="Aleksandar Bubalo - IT koordinator" />
                </div>
            </div>
            <div class="commentPanel">
                <div class="textPart">
                    <Comment text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Turpis euismod porta laoreet molestie id sed bibendum. Blandit facilisi bibendum et, ullamcorper ac. 
                    Habitasse elit tellus vitae nulla quisque blandit fermentum. Volutpat aenean volutpat diam vel, facilisi. Quam porttitor sed pellentesque in elementum lacus tellus. Mauris 
                    sed tellus quis mattis egestas viverra. Morbi netus in pellentesque laoreet duis massa.
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Turpis euismod porta laoreet molestie id sed bibendum. Blandit facilisi bibendum et, ullamcorper ac. 
                    Habitasse elit tellus vitae nulla quisque blandit fermentum. Volutpat aenean volutpat diam vel, facilisi. Quam porttitor sed pellentesque in elementum lacus tellus. Mauris 
                    sed tellus quis mattis egestas viverra. Morbi netus in pellentesque laoreet duis massa." who="Aleksandar Bubalo - IT koordinator"/>
                </div>
                <div class="imgComm">
                    <div class="arrowRight"></div>
                    <div class="imgPart">
                        <img src="../../assets/Bubalo.jpg" alt="Bubi gang" class="inImgPart">
                    </div>
                </div>
            </div>
            <div class="commentPanel">
                <div class="imgComm">
                    <div class="imgPart">
                        <img src="../../assets/Bubalo.jpg" alt="Bubi gang" class="inImgPart">
                    </div>
                    <div class="arrowLeft"></div>
                </div>
                <div class="textPart">
                    <Comment text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Turpis euismod porta laoreet molestie id sed bibendum. Blandit facilisi bibendum et, ullamcorper ac. 
                    Habitasse elit tellus vitae nulla quisque blandit fermentum. Volutpat aenean volutpat diam vel, facilisi. Quam porttitor sed pellentesque in elementum lacus tellus. Mauris 
                    sed tellus quis mattis egestas viverra. Morbi netus in pellentesque laoreet duis massa.  viverra. Morbi netus in pellentesque laoreet duis massa." who="Aleksandar Bubalo - IT koordinator"/>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import Comment from "../Comment.vue";

export default {
  name: "ToldAboutUs",
  components: {
    Comment
}
}
</script>

<style>

.toldAboutUs{
    position: relative;
    width: 100%;
    padding-top: 65px;
}

#sasChurch{
    margin: 400px auto;
    left: 12%;
    opacity: 0.5;
    position: absolute;
    width: 65vw;
}

#aboutUsTitle{
    margin: 0px;
    padding: 40px auto;
    text-align: center;
    font-size: 75px;
    color: #E52A30;
}

.commentPanels{
    width: 85%;
    margin: 10px auto;
    padding-bottom: 40px;
    opacity: 0.9;
}

.commentPanel{
    display: flex;
    justify-content: center;
}

.imgComm{
    display: flex;
    gap: 10px;
    /* margin-top: -25px; */
}

.imgPart{
    margin-top: 150px;
    background-color: #FE8A90;
    width: 350px;
    height: 350px;
    border-radius: 50%;
    display: flex;
    justify-content: center;
}

.inImgPart{
    margin: 25px auto;
    width: 300px;
    height: 300px;
    border-radius: 50%;
}

.textPart{
    display: flex;
    width: 70%;
    padding-bottom: 50px;
    position: relative;
}

.arrowLeft {
    clip-path: polygon(100% 0, 0% 100%, 100% 100%);
    width: 60px;
    height: 60px;
    background-color: #E52A30; 
    margin-top: 250px;
    box-shadow: 0 5px 12px rgb(0 0 0 / 16.1%);
}

.arrowRight {
    clip-path: polygon(0 0, 0% 100%, 100% 100%);
    width: 60px;
    height: 60px;
    background-color: #E52A30; 
    margin-top: 250px; 
    box-shadow: 0 5px 12px rgb(0 0 0 / 16.1%);
}

@media screen and (max-width: 1100px) {
    #aboutUsTitle{
        font-size: 7vw;
    }
    
    .imgPart{
        width: 30vw;
        height: 30vw;
    }

    .inImgPart{
        width: 24vw;
        height: 24vw;
    }

    .arrowLeft {
        width: 5vw;
        height: 5vw;
        margin-top: 70%;
    }

    .arrowRight {
        width: 5vw;
        height: 5vw;
        margin-top: 70%;
    }

    .imgPart{
        margin-top: 20vw;
        
    }
}

@media screen and (max-width: 700px) {
    #aboutUsTitle{
        font-size: 34px;
    }

    .imgComm{
        display: none;
        margin-top: 100px;
    }

    .textPart{
        padding-bottom: 0px;
        width: 85%;
    }
}


</style>