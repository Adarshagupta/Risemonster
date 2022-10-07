<body>


<div class="container">
    <h1>MUTANT ROADMAP</h1>
    <ul class="cards">
      <li class="card">
        <div>
            <div class="span">
                <div>Phase 01</div>
                <div class="spans">
                    <h4>0%</h4>
                </div> 
                </div>
          <h3 class="card-title">PLANNING</h3>
          <div class="card-content">
            <p>Quality comes first. We took our time to plan out everything and build our production pipeline for a good quality artwork.</p>
          </div>
        </div>
        
      </li>
      <li class="card">
        <div>
            <div class="span">
                <div>Phase 02</div>
            <div class="spans">
                <h4>25%</h4>
            </div> 
            </div>
          <h3 class="card-title">PRODUCTION</h3>
   
          <div class="card-content">
            <p>Starting the production on the procedurally genersted planets and smart contrsct for minting.</p>
    
        </div>
          
        </div>
  
      </li>
      <li class="card">
        <div>
            <div class="span">
                <div>Phase 03</div>
                <div class="spans">
      <h4>50</h4>

                </div> 
                </div>
          <h3 class="card-title">LAUNCH</h3>
          <div class="card-content">
            <p>Our most active community members well be able to join the whitelist so they can discover, collect and sell there NFTs.</p>
          </div>
        </div>

      </li>
      <li class="card">
        <div>
            <div class="span">
                <div>Phase 04</div>
                <div class="spans">
                    <h4>75%</h4>
                </div> 
                </div>
          <h3 class="card-title">MINTING</h3>
          <div class="card-content">
            <p>Pre-Sale Minting is opened for our whitelisted members.The price for ehitelist minting well be 2 SOL.</p>
          </div>
        </div>

      </li>
      <li class="card">
        <div>
            <div class="span">
                <div>Phase 05</div>
                <div class="spans">
                    <h4>80%</h4>
                </div> 
                </div>
          <h3 class="card-title">NEW NFTs</h3>
          <div class="card-content">
            <p>Typesetting industry when an unknown printer took a gallery of type and scrambled it to make a type specimen book.</p>
          </div>
        </div>
 
      </li>
      <li class="card">
        <div>
            <div class="span">
                <div>Phase 06</div>
                <div class="spans">
    <h4>100%</h4>
                </div> 
                </div>
          <h3 class="card-title">METAVERSE</h3>
          <div class="card-content">
            <p>A complete account of system, and expound the actual teachings of the great explorar of the truth.</p>
          </div>
        </div>
        
      </li>
     
    </ul>
  </div>
</body>
<style>
    :root {
  --orange: rgba(64, 67, 253, 0.522);
  --darkorange: #dd7d25;
  --black: #2b2d42;
  --white: #fff;
  --thumb: #edf2f4;
}

* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}
h1{
    color: yellow;
    font-weight: 900;
    display: flex !important;
    line-height: 1.2;
    font-size: 2.5em;

    font-family: "Montserrat",sans-serif;
}
.card-title{
    color: rgb(255, 72, 0);
    font-weight: 900;
    display: flex !important;
    line-height: 1.2;
    font-size: 2.5em;
    margin-top: 10px;
    

    font-family: "Montserrat",sans-serif;
}
body {
  font: 16px / 24px "Rubik", sans-serif;
  color: var(--black);
  background: var(--platinum);
  margin: 50px 0;
}


.container {
  max-width: 1400px;
  padding: 0 15px;
  margin: 0 auto;
}

h2 {
  font-size: 32px;
  margin-bottom: 1em;
  color: white;
}

.cards {
  display: grid;
  grid-auto-columns: 100%;
  grid-column-gap: 10px;
  grid-auto-flow: column;
  padding: 25px 0px;
  list-style: none;
  overflow-x: scroll;
  scroll-snap-type: x mandatory;
  border-radius: 20px;
}

.card {
  display: flex;
  flex-direction: column;
  padding: 20px;
  width: 350px;
  background: rgba(56, 76, 255, 0.384);
  border-radius: 12px;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 15%);
  scroll-snap-align: start;
  transition: all 0.2s;
  color: white;
  height: 400px;
  border: 2px solid yellow;
}

.card:hover {
  color: var(--white);
  background: var(--orange);
}

.card .card-title {
  font-size: 20px;
}

.card .card-content {
  margin: 20px 0;
  max-width: 85%;
}

.card .card-link-wrapper {
  margin-top: auto;
}

.card .card-link {
  display: inline-block;
  text-decoration: none;
  color: white;
  background: var(--orange);
  padding: 6px 12px;
  border-radius: 8px;
  transition: background 0.2s;
}

.card:hover .card-link {
  background: var(--darkorange);
}

.cards::-webkit-scrollbar {
  height: 12px;
}

.cards::-webkit-scrollbar-thumb,
.cards::-webkit-scrollbar-track {
  border-radius: 92px;
}

.cards::-webkit-scrollbar-thumb {
  background: var(--darkorange);
}

.cards::-webkit-scrollbar-track {
  background: var(--thumb);
}

@media (min-width: 500px) {
  .cards {
    grid-auto-columns: calc(50% - 10px);
    grid-column-gap: 20px;
  }
}

@media (min-width: 700px) {
  .cards {
    grid-auto-columns: calc(calc(100% / 3) - 20px);
    grid-column-gap: 30px;
  }
}

@media (min-width: 1100px) {
  .cards {
    grid-auto-columns: calc(30% - 0px);
    grid-column-gap: 40px;
  }
}


/* FOOTER STYLES
–––––––––––––––––––––––––––––––––––––––––––––––––– */
.page-footer {
  position: fixed;
  right: 0;
  bottom: 50px;
  display: flex;
  align-items: center;
  padding: 5px;
  z-index: 1;
}

.page-footer a {
  display: flex;
  margin-left: 4px;
}
.span{
    display: flex;
    justify-content: flex-end;
    justify-content: space-between;
margin: 5px;
padding: 5px;

}
.spans{
    width: 48px;
  height: 48px;
  display: flex;
  background: purple;
 display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding-top: 2px;
  line-height: 1;
  border-radius: 100%;
  transform: rotate(16deg);
  background: rgb(164,66,193);
background: linear-gradient(90deg, rgba(164,66,193,1) 0%, rgba(85,0,255,1) 97%, rgba(20,0,28,1) 100%); 
border-bottom: 1px solid #3b3b3b;

}
p{
    font-size: large;
}

</style>