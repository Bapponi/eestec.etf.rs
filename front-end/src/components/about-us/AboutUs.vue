<template>
    <div class="aboutUs">
        <img src="../../assets/ilustrations/genexR.png" alt="genex" id="genexAbout">
        <div class="aboutSection">
            <h2 class="aboutTitle">O nama</h2>
            <div>
                <p class="aboutText">Lokalni komitet Beograd je član Udruženja studenata elektrotehnike Evrope 
                    – Istek od 2000. godine i trenutno je, sa svojih više od 250 članova, 
                    jedan od najbrojnijih i najbolje organizovanih lokalnih komiteta u Evropi. 
                    Tokom godina postojanja, preko 800 studenata Elektrotehničkog fakulteta 
                    Univerziteta u Beogradu učestvovalo je na stručnim seminarima i kulturnim 
                    razmenama u gradovima širom Evrope.</p>
                <p class="aboutText">
                    Od osnivanja do danas, organizovali smo preko 80 međunarodnih i lokalnih događaja, 
                    sa ciljem da domaćim i stranim studentima pružimo priliku za stručno, lično i profesionalno 
                    usavršavanje i podstaknemo upoznavanje različitih kultura. Kroz dva Kongresa Udruženja, 
                    predsedničku konferenciju Udruženja, 8 stručnih radionica i 11 razmena, Beograd i Srbiju 
                    posetilo je oko 700 studenata iz 25 zemalja Evrope. O pozitivnoj slici naše zemlje i glavnog 
                    grada koju su u svoje domovine odneli strani studenti, najbolje svedoči to što se mnogi ponovo 
                    vraćaju da učestvuju na još nekom od naših događaja ili barem posete svoje kolege i učvrste 
                    stečena prijateljstva. Pri biranju teme za stručne radionice, vodimo se željom da studentima 
                    različitih oblasti elektrotehnike pružimo priliku da učestvuju na događaju i upoznaju se sa 
                    novim dostignućima u oblastima koje se sprovode na našem fakultetu.
                </p>
            </div>
        </div>
        <div class="aboutImage">
            <img class="okvir" src="../../assets/okvir.png" alt="okvir">
            <img class="aboutImg" src="../../assets/EC21.png" alt="ec21">
        </div>
        
    </div>
</template>

<style>

    .aboutUs{
        display: flex;
        justify-content: space-between;
        background-color: white;
    }

    .aboutSection{
        margin-top: 5%;
        width: 50%;
    }

    .aboutTitle{  
        margin: 0px;
        padding-bottom: 40px;
        padding: 40px auto;
        text-align: center;
        font-size: 45px;
        color: #E52A30;
    }

    .aboutText{
        text-align: center;
        margin: 10px 10%;
    }

    #genexAbout{
        height: 700px;
        position: absolute;
    }

    .aboutImg{
        height: 700px;
        opacity: 0.75;
    }

    .aboutImage{
        display: flex;
    }

    .okvir{
        position: absolute; 
        height: 700px;
        z-index: 2;
        margin-left: -125px;
        /* top: 100.05vh; */
    }

    @media screen and (max-width: 1260px) {
        .aboutImage{
            display: none;
        }

        .aboutUs{
            justify-content: center;
            
        }

        .aboutSection{
            width: 90%;
            margin-bottom: 7%;
        }

        #genexAbout{
            margin-top: 2%;
            height: 60%;
        }
    }

    @media screen and (max-width: 700px) {
        
        #genexAbout{
            margin-top: 5%;
            height: 75%;
        }
    }

</style>