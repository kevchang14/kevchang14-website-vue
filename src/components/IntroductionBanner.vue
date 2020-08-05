<template>
    <div class='introduction-banner'>
        <link href='https://fonts.googleapis.com/css?family=Andika' rel='stylesheet'>
        <div class='introduction-name'>
            Hey!
            <br>
            I'm Kevin
        </div>
    </div>
</template>

<script>
export default {
  name: 'IntroductionBanner',
}
</script>

<style scoped>
.introduction-banner {
    background-image: url('./../assets/img/introduction-background-w2500.jpg');
    background-position: 50% 50%;
    background-size: cover;
    height: 50vh;
    max-height: 60vw;
    text-align: center;
}
.introduction-name {
    display: flex;
    justify-content: center;
    flex-direction: column;
    height: 100%;
    font-family: 'Andika';
    font-size: 10vw;
    font-weight: bold;
    color: white;
}
</style>