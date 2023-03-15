<script>
export default{
    data(){
        return{
            items:[
                {
                    img: "../public/assets/sport1.png",
                    text:"MIXED MARTIAL ARTS",
                }, 
                {
                    img: "../public/assets/sport2.png",
                    text:"KICKBOXING",
                }, 
                {
                    img: "../public/assets/sport3.png",
                    text:"BRAZILIAN JIU-JITSU",
                }, 
                {
                    img: "../public/assets/sport4.png",
                    text:"KIDS CLASSES",
                }, 
           
            ]
        }
    }
}
</script>

<template>
<div className="imgContainer">


                        <div className="offeredItems" v-for="(item, index) of items"  :key=items.img  >
                            <img v-bind:src="item.img">
                            <p> {{ item.text }}</p>
                        </div>
                    </div>
                  

</template>

<style scoped>

.imgContainer{
    display:flex;
    justify-content: center;
    align-items: center;
    position:relative;
    color:white;
}

p{
    position:absolute;
}


img{
    width:24.79vw;
  -webkit-mask-image: -webkit-gradient(linear, left bottom, left top, color-stop(1%, rgba(0,0,0,1)), color-stop(80%, rgba(0,0,0,1)), color-stop(100%, rgba(0,0,0,0))), -webkit-gradient(linear, left top, right top, color-stop(0%, rgba(0,0,0,0)), color-stop(50%, rgba(0,0,0,1)), color-stop(100%, rgba(0,0,0,0)));
}

img:hover{
 transform: translate(0px,-10px);
 transition: 500ms;
 cursor:pointer
}


.offeredItems {
  display:flex;
    justify-content: center;
    align-items: center;
    position:relative;
    color:white;
    flex-direction: row;
}
.offeredItems > img {
position: relative;
}

.offeredItems > p{
    position: absolute;
  color: white;
  font-size: 1.5rem;
  font-weight: 900;
  font-family: 'Passion One', sans-serif;
  font-style:italic;
  margin: 0px;
  transform: scale(1, .8);
}
</style>