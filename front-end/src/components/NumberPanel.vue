<template>
    <div class="panels">
        <div class="panel">
            <div class="panelNumber">
                <p class="panelNumberText">22</p>
            </div>
            <div class="panelLabel">Godina postojanja</div>
        </div>
        <div class="panel">
            <div class="panelNumber">
                <p class="panelNumberText">300</p>
            </div>
            <div class="panelLabel">Članova udruženja</div>
        </div>
        <div class="panel">
            <div class="panelNumber">
                <p class="panelNumberText">120</p>
            </div>
            <div class="panelLabel">Organizovanih događaja</div>
        </div>
        <div class="panel">
            <div class="panelNumber">
                <p class="panelNumberText">100</p>
            </div>
            <div class="panelLabel">Partnerskih kompanija</div>
        </div>
    </div>
</template>

<style>
.panels{
    padding: 75px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 70px;
}

.panel{
    text-align: center;
    margin: 0px;
    min-width: 120px;
    width: 120px;
    height: 170px;
}

.panelNumber{
    display: flex;
    justify-content: center;
    align-content: center;
    border-radius: 10px;
    background-color:  #E52A30;
    height: 120px;
}

.panelNumberText{
    font-size: 37px;
    color: white;
}

.panelLabel{
    padding-top: 10px;
    font-size: 18px;
    text-align: center;
}
</style>