<template>
    <div class="logo-container">
        <svg id="Layer_1" viewBox="0 0 368.5 225.81" :style="{width, height}">
        <defs>
            <clipPath id="clip-path" transform="translate(-65.75 -66.94)">
                <rect class="cls-1" x="65.75" y="66.94" width="368.5" height="159.11"/>
            </clipPath>
        </defs>
        <text class="cls-2" :style="{'fill': color}" transform="translate(30.44 209.82)">LC Belgrade</text>
        <g class="cls-3">
            <path :style="{'fill': color}" d="M189.12,149.31a24,24,0,0,0-45.87,0Zm-47,6.94A24,24,0,0,0,184,172.19h9.84a31.88,31.88,0,1,1,4.27-15.94Z" transform="translate(-65.75 -66.94)"/>
            <path :style="{'fill': color}" d="M120.69,149.31a24,24,0,0,0-45.87,0Zm-46.95,6.94a24,24,0,0,0,41.88,15.94h9.82a31.87,31.87,0,1,1,4.28-15.94Z" transform="translate(-65.75 -66.94)"/>
            <path :style="{'fill': color}" d="M361,149.31a24,24,0,0,0-45.88,0ZM314,156.25a24,24,0,0,0,41.87,15.94h9.82A31.87,31.87,0,1,1,370,156.25Z" transform="translate(-65.75 -66.94)"/>
            <path :style="{'fill': color}" d="M277.56,172.16h0a8.15,8.15,0,0,0,8.09,8.21c9.14,0,16.84-2.56,19.14-6.05l4.61,5.35c-4.56,5-13.48,8.33-23.75,8.33a16,16,0,0,1-16-15.84h0l0-39.7v0H246.93V124.3h22.62V92.49h8V124.3h12.3v8.13H277.58l0,0v39.7Z" transform="translate(-65.75 -66.94)"/>
            <path :style="{'fill': color}" d="M374.42,156.2a32,32,0,0,1,59.83-15.8h-9.82a24,24,0,0,0-42,15.8v.05a24,24,0,0,0,41.86,15.94h9.84a32,32,0,0,1-59.69-15.94Z" transform="translate(-65.75 -66.94)"/>
            <path :style="{'fill': color}" d="M216.5,226c3.6-3,7.51-5.91,11.38-8.82,14.73-11.06,30-22.51,30-36.78s-15.2-25.63-29.9-36.67c-13.36-10-27.18-20.42-27.18-31.19s13.79-21,27.11-31.07A194.11,194.11,0,0,0,245.76,67l-10.39,0c-3.65,3-7.63,6-11.57,9-14.7,11-29.89,22.45-29.89,36.66s15.23,25.72,30,36.79c13.32,10,27.1,20.36,27.1,31.07s-13.81,21.15-27.18,31.19A197.44,197.44,0,0,0,206,226.05Z" transform="translate(-65.75 -66.94)"/>
        </g>
        </svg>
    </div>
</template>

<script>
export default {
    props: {
        width: Number,
        height: Number,
        color: String
    }
}
</script>

<style scoped>

    .cls-1 {
        fill: none;
    }

    .cls-2 {
        font-size: 52.14px;
        font-family: CenturyGothic-Bold, Century Gothic;
        font-weight: 700;
    }

    .cls-3 {
        clip-path: url(#clip-path);
    }

</style>