<script>
    import banner from "../assets/banner3.png";
</script>
<body class="body">
    <div>
    <h1>Mutant Metaverse</h1>
    <p>Ultimately, ROM aims to create an amazing playable experience for everyone, holders and non-holders alike. As we expand our team and move forward into development, we have one purpose in mind. Create the best game possible.</p>
    </div>
    <img class="img" src={banner} alt="" srcset="">
</body>
<style>
    @media only screen and (max-width: 800px) {
   
    .body{
        display: flex;
        justify-content: space-between;
        flex-direction: column;
        margin-top: 10px;
    margin-bottom: 40px;

    }
}
body{
    display: flex;
    justify-content: space-between;
    flex-direction: row;
    margin-top: 60px;
    margin-bottom: 60px;
    background-image: url("../assets/banner2.png");
    padding: 20px;
    background-size: cover;
    border-radius: 20px;
    border: 2px solid white;

 
}
    h1{
    color: yellow;
    font-weight: 900;
    display: flex !important;
    line-height: 1.2;
    font-size: 2.5em;
    text-shadow: 2ch;

    font-family: "Montserrat",sans-serif;
}
p{
    color: white;
    max-width: 500px;
    font-weight: bold;
}
img{
    max-width: 400px;
    border-radius: 20px;
    border: 2px solid white;
}
</style>