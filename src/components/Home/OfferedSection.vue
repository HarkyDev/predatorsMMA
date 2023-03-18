<script>
export default{
    data(){
        return{
            items:[
                {
                    img: "assets/sport1.png",
                    text:"MIXED MARTIAL ARTS",
                    index: 1,
                    route: "#/MIXED-MARTIAL-ARTS"
                }, 
                {
                    img: "assets/sport2.png",
                    text:"KICKBOXING",
                    index: 2,
                    route: "#/KICKBOXING"
                }, 
                {
                    img: "assets/sport3.png",
                    text:"BRAZILIAN JIU-JITSU",
                    index: 3,
                    route: "#/BRAZILIAN-JIU-JITSU"
                }, 
                {
                    img: "assets/sport4.png",
                    text:"KIDS CLASSES",
                    index: 4,
                    route: "#/KIDS-CLASSES"
                }, 
           
            ]
        }
    }
}
</script>

<template>
<div className="imgContainer">


                        <div className="offeredItems" v-for="(item, index) of items"  v-bind:key=index  >
                                <a v-bind:href="item.route">
                                    <p class="itemTitle"> {{ item.text }}</p>
                                    <div className="gradientOverlay"></div>
                                    <img v-bind:src="item.img">
                                </a>
                        </div>
                    </div>
                     <font-awesome-icon icon="fa-solid fa-user-secret" />
                  

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
    z-index: 2;
}
.gradientOverlay{
    background: linear-gradient(to bottom right, rgb(55, 55, 55), rgb(0, 0, 0));
    width: 100%;
    height: 100%;
    opacity: 0.4;
    position: absolute;
    z-index: 1;
}



img{
    width:24.79vw;

}

.gradientOverlay:hover {
    transition: 100ms;
    background: linear-gradient(to bottom right, rgb(255, 251, 0), rgb(113, 108, 0));
    cursor:pointer;
}

.gradientOverlay:hover + img{
    transition: 100ms;
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

.itemTitle{
    text-align: center;
    position: absolute;
    color: white;
    font-size: 170%;
  font-weight: 900;
  font-family: 'Passion One', sans-serif;
  font-style:italic;
  margin: 0px;
  transform: scale(1, .8);
}

a{
    display: flex;
    align-items: center;
    justify-content: center;
}

</style>