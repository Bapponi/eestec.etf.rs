<template>
    <div class="nav">
        <div class="logo">
            <Logo width="150px" height="150px" color="#fff"/>
        </div>
        <div id="nav-bar" class="inner">
            <div class="menu">
                <ul class="menu__list">
                    <li><a href="/">Početna</a></li>
                    <li><a href="/about">O nama</a></li>
                    <li><a href="">Vesti</a></li>
                    <li><a href="">Projekti</a></li>
                    <li><a href="">Partneri</a></li>
                    <li><a href="">Kontakt</a></li>
                </ul>
            </div>
            <div class="buttons">
                <Button class="button">Učlani se</Button>
                <Button class="button">Uloguj se</Button>
            </div>
        </div>
        <div class="icon" @click="toggleNav">
            <!-- <img src="../assets/bar.svg" alt="nav" style="color: white"> -->
            <div class="bar"></div>
            <div class="bar"></div>
            <div class="bar"></div>
        </div>
    </div>
</template>

<script>
import Logo from "@/components/Logo.vue"
import Button from "@/components/Button.vue"

export default {
    name: 'Nav',
    components: {
        Logo,
        Button
    },
    methods: {
      toggleNav (event) {
        console.log("Kliknuto!");
        var x = document.getElementById("nav-bar");
        if (x.className === "inner") {
            console.log("Usao inner");
            x.className += " responsive";
        } else {
            console.log("Usao responsive");
            x.className = "inner";
        }
      }
  }
}
</script>

<style scoped>

.nav {
    left: 0px;
    background: #990008;
    z-index: 2;
    height: 153px;
    /* position: absolute; */
    /* width: 100vw; */
    transition: transform 0.2s;
}

.inner {
    padding-top: 50px;
    margin: 0 auto;
    display: flex;
    align-items: center;
    gap: 55px;
    justify-content: right;
    width: 92%;
}
.menu__list {
    display: flex;
    list-style: none;
    gap: 30px;
    color: white;
    font-size: 18px;
}
.menu__list a{
    color: white;
    text-decoration: none;
}

.menu__list a:hover{
    color: white;
    border-bottom: 2px solid white;
    transition: 0.2s;
}

.buttons {
    display: flex;
    gap: 30px;
}

.logo{
    padding-left: 75px;
    position: absolute;
    z-index: 3;
}

.icon{
    display: none;
    width: 50px;
    position: absolute;
    right: 55px;
    top: 50px;
}

.bar{
    width: 50px;
    height: 5px;
    background-color: white;
    margin-bottom: 10px;
}

@media screen and (max-width: 1100px) {
    .inner .menu {display: none;}

    .inner .buttons {display: none;}

    .icon {
      float: right;
      display: block;
    }

    .inner.responsive {
        position: absolute;
        height: 100vh;
        width: 100%;
        background-color: #990008;
        opacity: 0.9;
        justify-content: center;
        padding-top: 0px;
        flex-direction: column;
    }

    .inner.responsive .menu {
        display: block;
        padding-top: 135px;
    }

    .menu__list{
        flex-direction: column;
        font-size: 20px;
    }

    .inner.responsive .buttons {
        display: block;
        flex-direction: column;
        gap: 30px;
        padding-left: 50px;
    }

    .button {
        margin-bottom: 30px;
    }

    .inner.responsive a {
        float: none;
        display: block;
        text-align: left;
    }
}

</style>