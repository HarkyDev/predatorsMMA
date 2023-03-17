<script>
</script>

<template>
      <div className="navBarWrapper">

            <img src="public\assets\logo-w.png" alt="" height="100" /> 
            <div className="textWrapper">
                  <p className="navBarButtons">HOME</p>
                  <p className="navBarButtons">ABOUT</p>
                  <p className="navBarButtons">CLASSES</p>
                  <p className="navBarButtons">CONTACT</p>
                  <p className="navBarButtons">REVIEWS</p>
                  <div className="callUsDiv">
                        <p>CALL US</p>
                        <p>07897313488</p>

                  </div>

            </div>
      </div>

</template>


<style scoped>

.navBarButtons:hover{
      transition: 0.5s;
      color: white;
      cursor: pointer;
}
.callUsDiv{
      text-align: right;
display: flex;
flex-direction: column;
justify-content: right;
}
p{
       font-weight: 500;
  text-align: center;
  font-size: 1rem;
  font-weight: 700;
  color: yellow;
  font-family: 'Passion One', sans-serif;
  font-style:italic;
  margin-right: 30px;
}

.textWrapper:hover >{
      transition: 0.5s;
      color: white;
      cursor: pointer;
}

.textWrapper{
      display: flex;
      flex-direction: row;
}




.navBarWrapper{
      background-color: rgb(0, 0, 0);
      padding: 10px;
      display: flex;
      flex-direction: row;
      justify-content: space-around;
      align-items: center;
}


</style>