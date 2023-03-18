
<script setup>

import { Icon } from '@iconify/vue'


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
          <div className="socialsContainer">
            <a className="socialLink">
              <Icon className="socialIcon" icon="mdi:instagram"/>
            </a>
            <a className="socialLink">
              <Icon className="socialIcon" icon="mdi:youtube"/>
            </a>
            <a className="socialLink">
              <Icon className="socialIcon" icon="mdi:twitter"/>
            </a>
            <a className="socialLink">
              <Icon className="socialIcon" icon="mdi:facebook"/>
            </a>
          
        </div>
  </div>
</template>


<style scoped>

.socialsContainer{
  display: flex;
  margin-top: 10rem;
  min-width: 10%;
  justify-content: space-around;
  color: yellow;
  font-size: 1.3rem;
}

.socialLink {
  color: yellow;
  cursor: pointer;
}
.socialLink:hover {
  transition: 500ms;
  color: white;
  cursor: pointer;
  background: none;
  font-size: 1.5rem;
}

.socialLink:hover + .socialIcon{
  transition: 500ms;
}



.hero-bg{
  background-image: url("public/assets/bg.png");
  background-repeat: repeat-y;
  width: 99vw;
  min-height: 96vh;
  display:flex;
  flex-direction: column;
  align-items:center;
  justify-content: center;
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  top:0px;
  left:0px;
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
  padding: 1rem 2rem;
  border-radius: 1rem;
  font-weight: 900;
  font-family: 'Passion One', sans-serif;
  background-color:yellow;
  box-shadow: 0px 0px 100px yellow;
  margin-top: 8rem;
  font-style:italic;
}

button:hover{
  box-shadow: 0px 0px 120px yellow;
  transition: 500ms;
  cursor:pointer;
  transform: scale(1.1)
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
