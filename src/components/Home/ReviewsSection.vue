<script >



export default {
  data() {
    return {
      items: [
        {
          img: 'assets/review1.png',
          name: 'Sally James',
          text: 'I recently joined Predators MMA gym and I have to say, it has been an amazing experience! The trainers are incredibly knowledgeable and supportive, always pushing me to be my best. ',
          stars: 5,
        },
        {
          img: 'assets/review2.png',
          name: 'John Stewart',
          text: "Predators MMA gym is the real deal! The trainers are extremely experienced and knowledgeable, and they really know how to push you to your limits.",
          stars: 5,
        },
        {
          img: 'assets/review3.png',
          name: 'Rachel Roth',
          text: "I've been training at Predators for a few months now, and I've seen amazing progress in my fitness level and technique. The facilities are clean and modern, and the equipment is top-notch.",
          stars: 5,
        },
        {
          img: 'assets/review4.png',
          name: 'Bobby Drake',
          text: 'What I love most about Predators is the sense of community. Everyone is so friendly and supportive, and the training sessions are always a blast.',
          stars: 5,
        },
        {
          img: 'assets/review5.png',
          name: 'Dick Grayson',
          text: 'The instructors at Predators really take the time to teach proper form and technique, which has helped me avoid injury and make significant gains in strength and endurance.',
          stars: 4,
        },
        {
          img: 'assets/review7.png',
          name: 'James Howlett',
          text: "I've trained at a lot of gyms over the years, but Predators is by far the best.The trainers are passionate about what they do, and it shows in every session.",
          stars: 4,
        },
        {
          img: 'assets/review6.png',
          name: 'Natasha Romanoff',
          text: "If you're serious about MMA or just want to get in shape, Predators is the place to be.The atmosphere is electric, and the trainers will push you to be your best",
          stars: 5,
        },
        {
          img: 'assets/review8.png',
          name: 'Dianna Prince',
          text: "I can't recommend Predators enough! The training is intense, but the results are worth it. Plus, the community is amazing and supportive, making it a great place to train and make friends.",
          stars: 5,
        },
      ]
    }
  }
}
</script>

<template>
  <div className="reviewSection">

    <div className="reviewContainer">
      <div className="reviewItems" v-for="(item, index) of items" v-bind:key="index">
        <div className="cardContainer">
                <img v-bind:src="item.img"/>
                <p className="userName">{{ item.name }}</p>
                <div className="starsContainer">
                  <p v-bind:v-for="n in item.stars"> 
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path fill="currentColor" d="m12 18.275l-4.15 2.5q-.275.175-.575.15q-.3-.025-.525-.2q-.225-.175-.35-.437q-.125-.263-.05-.588l1.1-4.725L3.775 11.8q-.25-.225-.312-.513Q3.4 11 3.5 10.725q.1-.275.3-.45q.2-.175.55-.225l4.85-.425l1.875-4.45q.125-.3.388-.45q.262-.15.537-.15t.538.15q.262.15.387.45l1.875 4.45l4.85.425q.35.05.55.225q.2.175.3.45q.1.275.038.562q-.063.288-.313.513l-3.675 3.175l1.1 4.725q.075.325-.05.588q-.125.262-.35.437q-.225.175-.525.2q-.3.025-.575-.15Z"/></svg>
                  </p>
                </div>
                <p className="userText">"{{ item.text }}""</p>
              </div>
              
              
            </div>
          </div>
        </div>
</template>

<style scoped>
.reviewSection{
  padding: 50px;
}
.userText{
  text-align: center;
  color: white;
   font-size: 1rem;
  font-weight: 700;
  font-family: 'Passion One', sans-serif;
  font-style:italic;
  margin: 0px;
}
.userName{
   color: white;
 font-size: 1rem;
  font-weight: 900;
  font-family: 'Passion One', sans-serif;
  font-style:italic;
  margin: 0px;

}
svg{
  color: yellow;
}
.reviewItems{
  flex: 0 0 auto; 
  width: 300px;
}
.reviewSection{
  display: flex;
  align-items: center;
  justify-content: center;
}
.starsContainer{
    display: flex;

}
.cardContainer{
    display: flex;
    height: 100%;
    flex-direction: column;
    align-items: center;
    justify-content: top;
    padding: 20px 50px;
    background-color: rgb(1,1,1,0.1);
    border-radius: 20px;
    margin:20px;
    flex: 0 0 auto; 
  }
  
  
  .reviewContainer {
    
    width: 60vw;
    display: flex;
    flex-wrap: nowrap;
    overflow-x: hidden;
    overflow-y: hidden;
    -webkit-overflow-scrolling: touch;
    -webkit-scrollbar { display: none; }
}

img{
  width: 128px;
  height: 128px;
  object-fit: cover;
  border-radius: 50%;
}





</style>
