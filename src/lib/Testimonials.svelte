<script>

function stopAnimation() {
    document.querySelector('.slider .slide-track').style.animationPlayState = 'paused';
}

function startAnimation() {
    document.querySelector('.slider .slide-track').style.animationPlayState = 'running';
}

</script>
<body>
    
<div class="slider" on:mouseover={stopAnimation} on:mouseout={startAnimation}> Check out our partners
<div class="slide-track" on:mouseover={stopAnimation} on:mouseout={startAnimation}>
<div class="slide">
    <img src="https://crypto-central.io/library/uploads/Messari-Logo.png" height="100" width="100" alt="">
</div>
<div class="slide">
    <img src="https://crypto-central.io/library/uploads/Messari-Logo.png" height="100" width="100" alt="">
</div>
<div class="slide">
    <img src="https://crypto-central.io/library/uploads/Messari-Logo.png" height="100" width="100" alt="">
</div>
<div class="slide">
    <img src="https://crypto-central.io/library/uploads/Messari-Logo.png" height="100" width="100" alt="">
</div>
<div class="slide">
    <img src="https://crypto-central.io/library/uploads/Messari-Logo.png" height="100" width="100" alt="">
</div>
<div class="slide">
    <img src="https://crypto-central.io/library/uploads/Messari-Logo.png" height="100" width="100" alt="">
</div>
<div class="slide">
    <img src="https://crypto-central.io/library/uploads/Messari-Logo.png" height="100" width="100" alt="">
</div>
<div class="slide">
    <img src="https://crypto-central.io/library/uploads/Messari-Logo.png" height="100" width="100" alt="">
</div>
<div class="slide">
    <img src="https://crypto-central.io/library/uploads/Messari-Logo.png" height="100" width="100" alt="">
</div>
<div class="slide">
    <img src="https://crypto-central.io/library/uploads/Messari-Logo.png" height="100" width="100" alt="">
</div>
<div class="slide">
    <img src="https://crypto-central.io/library/uploads/Messari-Logo.png" height="100" width="100" alt="">
</div>
<div class="slide">
    <img src="https://crypto-central.io/library/uploads/Messari-Logo.png" height="100" width="100" alt="">
</div>
<div class="slide">
    <img src="https://crypto-central.io/library/uploads/Messari-Logo.png" height="100" width="100" alt="">
</div>
<div class="slide">
    <img src="https://crypto-central.io/library/uploads/Messari-Logo.png" height="100" width="100" alt="">
</div>
</div>
</div>

</body>

<style>

body {
    align-items: center;
    justify-content: center;
    margin-top: 40vh;
}

@keyframes scroll {
    0% {
        transform: translateX(0);
    } 100% {
        transform: translateX(calc(-250px * 7));
    }
}

.slider {
    text-align: center;
    background-color: #0C2520;
    height: 150px;
    margin: auto;
    overflow: hidden;
    position: relative;
    width: auto;
}

.slider .slide-track {
    animation: scroll 20s linear infinite;
    display: flex;
    width: calc(250px * 14);
}

.slider .slide {
    height: 100px;
    width: 250px;
}

.slide {
    cursor: pointer;

}
</style>