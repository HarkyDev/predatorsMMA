<script >



export default {
    data() {
        return {
            items: [
                {
                    img: 'https://i.gyazo.com/2078e59d193a8daa90520a792e51f85b.jpg',
                    name: 'Brendan Loughnane',
                    school: "Striking/Muay Thai"
                },
                {
                    img: 'https://mn2s-content.s3.eu-west-2.amazonaws.com/wp-content/uploads/2020/06/16162820/Jordan-Burroughs-MN2S.jpg',
                    name: 'Jordan Burroughs',
                    school: "Wrestling/Grappling"
                },
                {
                    img: 'https://cdn.shopify.com/s/files/1/1800/2299/articles/gordon-ryan-bjj-fanatics_1024x1024.jpg?v=1606926518',
                    name: 'Gordon Ryan',
                    school: "Brazilian Jiu-Jitsu"
                },
             
                {
                    img: 'https://i.gyazo.com/4ac054e4a2692d317617fa315036a1cb.jpg',
                    name: 'Max Holloway',
                    school: "Striking/Boxing"
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
                    <img v-bind:src="item.img" />
                    <div className="infoContainer">

                        <p className="userName">{{ item.name }}</p>
                        <p className="userText">{{ item.school }}</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>


.reviewContainer {
    background-color: rgb(1, 1, 1, 0.1);
    color: white;
    display: flex;
    justify-content: center;
    padding-top: 40px;
}
.cardContainer{
    background-color: rgb(0, 0, 0, 0.1);
    margin: 20px;
    padding-bottom: 30px;
    display: flex;
    flex-direction: column;
    align-items: center;
      border-radius: 20px;
    padding: 2rem;
}

.cardContainer:hover{
    transform: scale(1.1);
    transition: 400ms ease-in-out;
    cursor: pointer;
    background-color: rgba(199, 199, 199, 0.1);
    
}

img{
      border-radius: 20px;
      aspect-ratio: 1/1;
      width: 15vw;
}

.userName{
font-size: 1.5rem;
font-weight: 900;
}

.userText{
font-size: 1rem;
font-style: italic;
}



.infoContainer{
    display: flex;
    flex-direction: column;
    margin-top: 20px;
    justify-content: center;
    align-items: center;
  

}
</style>
