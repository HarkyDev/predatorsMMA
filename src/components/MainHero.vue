<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>


<template className="templateHero">
  <div className="hero-bg">
        <div class="greetings">
      <h1>
       PREDATORS <span className="span-h1">MMA</span>
      </h1>
      <h2>MIXED MARTIAL ARTS<span className="span-h2"> & BRAZILIAN JIU-JITSU</span></h2>
      </div>
      <button>BOOK A FREE CLASS</button>
  </div>
</template>


<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Rubik:wght@400;500;900&display=swap');


*{
  text-align: center;
  font-family:
}

.hero-bg{
  background-image: url("public/assets/bg.png");
  min-width: 100vw;
  min-height: 96vh;
  display:flex;
  flex-direction: column;
  align-items:center;
  justify-content: center;
}

h1 {
  font-weight: 500;
  text-align: center;
  font-size: 8rem;
  font-weight: 900;
  color: yellow;
  font-family: 'Passion One', sans-serif;
  font-style:italic;
  margin: 0px;
  transform: scale(1, .7);
  letter-spacing: -0.6rem;

}
.span-h1{
  color: white;
 font-size: 8rem;
  font-weight: 900;
  font-family: 'Passion One', sans-serif;
  font-style:italic;
  margin: 0px;
  transform: scale(1, .8);
  letter-spacing: -0.6rem;
}
h2 {
  font-weight: 500;
  text-align: center;
  font-size: 1.5rem;
  font-weight: 900;
  color: white;
  font-family: 'Passion One', sans-serif;
  font-style:italic;
  margin-top: -4rem;
  letter-spacing: 0.6rem;

}

.span-h2{
  color: yellow;
  font-weight: 500;
  text-align: center;
  font-size: 1.5rem;
  font-weight: 900;
  font-family: 'Passion One', sans-serif;
  font-style:italic;
  margin-top: -4rem;
  letter-spacing: 0.6rem;
}



h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

button{
  border:none;
  padding: 1rem;
  border-radius: 1rem;
  font-weight: 900;
  font-family: 'Passion One', sans-serif;
  background-color:yellow;
  box-shadow: 0px 0px 100px yellow;
  margin-top: 8rem;
  font-style:italic;
}

button:hover{
  box-shadow: 0px 0px 140px yellow;
  transition: 1s;
  cursor:pointer;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
