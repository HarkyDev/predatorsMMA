<template>
<div className="aboutContainer">
<div className="imgContainer">
    <img src="public\assets\about1.jpg">
</div>
        <div className="textContainer">
        <h2>
        IMPROVE FLEXIBILITY, BALANCE AND STRENGTH
        </h2>
        <h3>
        GET FIT WHILE LEARNING MARTIAL ARTSGET FIT WHILE LEARNING MARTIAL ARTS
        </h3>
        <p>
        Learn self-defense, build confidence, and get in the best shape of your life!
        Martial arts has tons of physical, mental and social benefits, suitable for anyone and everyone.
        Become part of something positive and learn new skills from trained martial arts professionals.
        It’s easy to get started - Book a FREE martial arts class today!
        </p>
        </div>
</div>
</template>

<style scoped>

.aboutContainer{
    display:flex;
    max-width: 90vw;
    margin-left: auto;
    margin-right: auto;
    
}

.aboutContainer > *{
   color: white;

}
.textContainer{
    max-width:40rem;
    padding: 4rem 0rem;
}

.imgContainer{
    padding: 4rem;
}

h2{
    font-weight:700;
    font-size: 2rem;
}
h3{
    font-size: 1.2rem;
    color:yellow;
    margin-bottom:2rem;
}

p {
    font-size: 1.4rem;
}
</style>