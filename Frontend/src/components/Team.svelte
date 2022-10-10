<script>
    import Avatar1 from "../assets/avatar1.png";
    import Avatar2 from "../assets/avatar2.png";
    import Avatar3 from "../assets/avatar3.png";
</script>
<body class="body">
 <div>
    <h1>The Team</h1>
    <p>Rise Of Mutants has been created by group of  blockchain enthusiasts.</p>
    <p><b>ADARSH:</b> Blockchain Developer, likes to work a lot.</p>
    <p><b>Prazzwol:</b> Artist, likes to waste time a lot</p>
    <p><b>Dolly: </b>Artist, Illutrator, loves technology besicly a nerd</p>
    <button>Join Team</button>
</div>
<div class="img">
<img src={Avatar1} alt="Avatar 1">
<img src={Avatar2} alt="Avatar 2">
<img src={Avatar3} alt="Avatar 3">
</div>

</body>
<style>
    body{
        color: white;
        display: flex;
        justify-content: center;
        
    }
    b{
        color: orangered;
    }
    h1{
    color: yellow;
    font-weight: 900;
    display: flex !important;
    line-height: 1.2;
    font-size: 2.5em;

    font-family: "Montserrat",sans-serif;
}
img{
    width: 130px;
    gap: 10px;

}
.img{
    margin-top: 40px;
    margin-bottom: 5px;
}
@media (min-width: 850px){
    .img{
        margin-top: 100px;
        margin-left: 100px;

    }

  }
  button{
    width: 200px;
    height: 40px;
    background-color: yellow;
    border-radius: 10px;
    font-weight: bold;
    font-size: large;
    border: 2px solid white;
  }
  button:hover{
    background-color: orangered;
    color: white;
    border: 2px solid yellow;
  }


</style>