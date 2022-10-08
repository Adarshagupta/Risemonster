<script>
    import logo from "../assets/logo.png"
    import romm1 from "../assets/romm1.png"
    import romm2 from "../assets/romm2.png"
    import romm3 from "../assets/romm3.png"
    import romm4 from "../assets/romm4.png"
    import romm6 from "../assets/romm6.png"
    import logosvg from "../assets/logo.svg"
    import Scroll from "../components/scroll.svelte";
    import fav from "../assets/favicon.png";
    import banner1 from "../assets/banner1.png"
    import Tools from "../components/tools.svelte";
    import logo1 from "../assets/logo1.svg"
    import Team from "../components/Team.svelte";
    import Footer from "../components/footer.svelte";
    import Fair from "../components/fair.svelte";
    import Faq from "../components/faq.svelte";
    import Join from "../components/join.svelte";

</script>

<body>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>ROM ~ Home</title>
    <link rel="stylesheet" href="global.css">
    <link rel="stylesheet" href="build/bundle.css">
    <link rel="icon" type="image/png" href={fav}>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
  </head>
<header>
    <div class="logo">
      <img class="logo-1" src={logo1} width="100px" alt="logo">
    </div>
    <div class="image1"> <img class="image-1" src={banner1} width="100px" alt="logo"></div>
</header>
<div class="row">
    <div class="text-1">
    <h1 class="h1">
      WELCOME TO 
      <br>
      RISE OF MUTANTS
    </h1>
    <p>
        Rise Of Mutants is collection of 4444 mutant monsters living in solana blockachain. Every Mutants are uniquely generated using ArtificiaL INtellegence
        BAYC is a collection of 10,000 Bored Ape NFTs—unique digital collectibles living on the Ethereum blockchain. Your Bored Ape doubles as your Yacht Club membership card, and grants access to members-only benefits
    </p></div>
<div class="image-2-section">
    <dev class="column">
        <img class="image3" src={romm1} alt="" srcset="">
    </dev>
    <dev class="column">
        <img class="image3" src={romm2} alt="">
    </dev>
    <dev class="column">
        <img class="image3" src={romm3} alt="">
    </dev>
    <dev class="column">
        <img class="image3" src={romm4} alt="">
        
    </dev>
</div>
</div>
<Fair />
<div class="box-info">
  <div>
    <img class="logosvg" src={logosvg} alt="svgicon" srcset="">
  </div>
    <div class="box-text">
      <p>Buy Rise of Mutants<br>
      in opensea or Rairable</p>
    </div>
    <div class="button">
      <button class="button1">BUY NOW</button>
    </div>
</div>
<div class="row">
    <div class="text-1">
    <h1 class="h1">
      THE UNIQUENESS OF MUTANTS
    </h1>
    <p>
        Rise Of Mutants is collection of 4444 mutant monsters living in solana blockachain. Every Mutants are uniquely generated using ArtificiaL INtellegence
        BAYC is a collection of 10,000 Bored Ape NFTs—unique digital collectibles living on the Ethereum blockchain. Your Bored Ape doubles as your Yacht Club membership card, and grants access to members-only benefits
    </p></div>
<div class="image-2-section">
    <dev class="column">
        <img class="image-4" src={romm6} alt="" srcset="">
    </dev>

</div>
</div>
<section>
   <Scroll />
</section>
<Tools />
<Team />
<Join />
<Footer />
</body>
<style>
    @import url('https://fonts.googleapis.com/css2?family=Noto+Sans&display=swap');
    body{
        font-family: 'Noto Sans', sans-serif;
    }
    @media ( min-width: 800px){
        body{
        margin-left: 60px;
        margin-right: 60px;
        }
    }
    .logo-1{
        max-width: 10%;
        max-width: 125px;
    width: auto;
    height: auto;
    }
    .logo{
        display: flex;
        justify-content: center;
        align-items: center;
        margin-top: 20px;
    }
    .image1{
        display: flex;
        justify-content: center;
        align-items: center;
        margin-top: 20px;
    }
  .image-1{
    max-width: 100%;
    width: 1200px;
    display: flex;
    justify-content: center;
    border-radius: 10px;
    border: 2px solid purple;


  }
  .row{
    display: flex;
    flex-direction: row;
    color: white;
    margin-top: 30px;
    
  }
  @media (max-width: 850px){
    .row{
      flex-direction: column;
    }
  }
h1{
    color: yellow;
    font-weight: 900;
    display: flex !important;
    line-height: 1.2;
    font-size: 2.5em;

    font-family: "Montserrat",sans-serif;
}
p{
    font-family: "Montserrat",sans-serif;
    font-size: 1.1em;
}
  .text-1{
    max-width: 600px;
  }
  .image-2-section{
    max-width: 100%;
    max-width: 400px;
    
  }
  @media(min-width: 850px){
    .image-2-section{
      margin-left: 90px;
    }
  }
  .image3{
    width: 160px;
    margin: 5px;
    border-radius: 10px;
    margin-left: 15px;
  }
  .box-info{
    width: 100%;
    height: 100px;
    background-color: yellow;
    border-radius: 10px;
    margin-top: 20px;
    display: flex;
    justify-content: space-between;
    
  }
.button1{
    background-color: purple;
    color: white;
    border: none;
    border-radius: 10px;
    padding: 10px;
    font-size: 1.2em;
    font-family: "Montserrat",sans-serif;
    margin-right: 20px;
}
.button1:hover{
    background-color: #3b3b3b;
    color: yellow;
}
  .logosvg{
    max-width: 100px;
  }
  .box-text{
    margin-left: 20px;
    margin-top: 10px;
    display: flex;
    justify-content: center;
    align-items: center;
    justify-content: space-around;
  }
  .button{
    display: flex;
    align-items: center;
    justify-content: flex-end;

  }
  .image-4{
    width: 100%;
    border-radius: 10px;
  }
  </style>
