<template>
    <div className="aboutContainer">
       
        <div className="imgContainer">
            <img src="https://i.gyazo.com/8d3348bcdb35ab190dc3fe36280213f3.png">
        </div>
        <div className="textContainer">
            <h2>
                Come Find Us here and get started
            </h2>
             <button>BOOK A FREE CLASS</button>
          
        </div>
    </div>
</template>

<style scoped>
img {
    width: 30vw;
}


.imgContainer:hover{
    cursor: pointer;
    transition: 300ms ease-in-out;
    transform: scale(1.05);
    animation: shake 0.5s;
    
}
.aboutContainer {
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: rgb(1, 1, 1, 0.15);
    width: 100%;

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

h1 {
    font-size: 1.2rem;
    color: yellow;
    margin-bottom: 2rem;
    font-weight: 900;
}

p {
    font-size: 1.4rem;
}

button{
  border:none;
  padding: 1rem 2rem;
  border-radius: 1rem;
  font-weight: 900;
  font-family: 'Passion One', sans-serif;
  background-color:yellow;
  margin-top: 8rem;
  font-style:italic;
}

button:hover{
  box-shadow: 0px 0px 20px -4px yellow;
  transition: 500ms;
  cursor:pointer;
  transform: scale(1.1)
}
</style>