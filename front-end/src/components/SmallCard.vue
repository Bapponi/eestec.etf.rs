<template>
    <div class="card-container">
        <div class="inner">
            <h2 class="title">{{ title }}</h2>
            <p class="text">{{ text }}</p>
            <p class="more">{{ more }}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: "SmallCard",
    props: {
        title: String,
        text: String,
        more: String,
        link: String
    }
}
</script>

<style scoped>

    .card-container {
        background-color: white;
        display: grid;
        place-items: center;
        position: relative;
        width: 400px;
        aspect-ratio: 1.2;
        box-shadow: 0 5px 12px rgb(0 0 0 / 16.1%);
        border-radius: 35px;
        opacity: 0.9;
    }

    .inner {
        max-width: 88%;
        position: relative;
        height: 95%;
        display: flex;
        align-items: center;
    }

    .title {
        position: absolute;
        top: 0;
        left: 0;
        font-size: 28px;
        color: #990008;
    }

    .text {
        max-width: 90%;
        font-size: 18px;
        line-height: 1.4;
    }

    .more {
        position: absolute;
        bottom: 0;
        right: 0;
        color: #990008;
        font-weight: bold;
        font-size: 18px;
    }

</style>