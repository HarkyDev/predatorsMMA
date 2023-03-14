<template>
<div className="imgContainer">
 <img src="public\assets\sport1.png" /> 
 <p>MIXED MARTIAL ARTS</p>
 <img src="public\assets\sport2.png" /> 
 <p>KICKBOXING</p>
 <img src="public\assets\sport3.png" />
 <p>BRAZILIAN JIU-JITSU</p> 
 <img src="public\assets\sport4.png" /> 
 <p>KIDS CLASSES</p>
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
</style>