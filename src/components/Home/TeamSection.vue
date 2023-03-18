<template>
    <div className="aboutContainer">
        <div className="textContainer">
            <h2>
                GAVIN BOARDMAN
            </h2>
            
            <p>
                Learn self-defense, build confidence, and get in the best shape of your life!
                Martial arts has tons of physical, mental and social benefits, suitable for anyone and everyone.
                Become part of something positive and learn new skills from trained martial arts professionals.
                It’s easy to get started - Book a FREE martial arts class today!
            </p>
        </div>
        <div className="imgContainer">
            <img src="public\assets\staff1.jpg">
        </div>
    </div>
</template>

<style scoped>


img{
     width: 30vw;
}
.aboutContainer {
    display:flex;
     align-items: center;
    justify-content: center;
    width:100%;


}

.aboutContainer>* {
    color: white;
}

.textContainer {
    max-width: 40rem;
    padding: 4rem 0rem;
}

.imgContainer {
    padding: 4rem;
}

h2 {
    font-weight: 700;
    font-size: 2rem;
}

h3 {
    font-size: 1.2rem;
    color: yellow;
    margin-bottom: 2rem;
}

p {
    font-size: 1.4rem;
}
</style>