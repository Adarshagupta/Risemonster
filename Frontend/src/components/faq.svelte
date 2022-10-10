<script>
console.clear();
// var element = document.getElementById("slide-menu");
// element.addEventListener("animationstart", listener, false);
// element.addEventListener("animationend", listener, false);
// element.addEventListener("animationiteration", listener, false);

// function listener(event){
//   console.log(event.elapsedTime)
// }

var isAnimating = false;
var isOpen = false;
var button = document.querySelector(".sticky-menu-container .outer-button");
var menu = document.querySelector(".sticky-menu-container .inner-menu");
var closeIcon = document.querySelector(".sticky-menu-container .outer-button .close-icon");
var arrowIcon = document.querySelector(".sticky-menu-container .outer-button .arrow-icon");
var menuItems = document.querySelectorAll(".sticky-menu-container .inner-menu > .menu-list > .menu-item");

var itemTexts = document.querySelectorAll(".sticky-menu-container .inner-menu > .menu-list > .menu-item > .item-text");

button.addEventListener("click", function(){
  if(isAnimating) return;
  this.classList.add("clicked");
  menu.classList.toggle("closed");
  
  if(isOpen){
    closeIcon.classList.remove("show");
    closeIcon.classList.add("hide");
    arrowIcon.classList.remove("hide");
    arrowIcon.classList.add("show");
    menuItems.forEach(function(item){
      console.log(item);
       item.classList.add("text-hides");
    });
    itemTexts.forEach(function(text, index){
        setTimeout(function(){
          text.classList.remove("text-in");
        });
    });
    isOpen = false;
  }
  else{
    closeIcon.classList.remove("hide");
    closeIcon.classList.add("show");
    arrowIcon.classList.remove("show");
    arrowIcon.classList.add("hide");
    menuItems.forEach(function(item){
      console.log(item);
       item.classList.remove("text-hides");
    });
    itemTexts.forEach(function(text, index){
        setTimeout(function(){
          text.classList.add("text-in");
        }, index*150);
    });
    isOpen = true;
  }
  
});

button.addEventListener("animationstart", function(event){
  isAnimating = true;
});

button.addEventListener("animationend", function(event){
  isAnimating = false;
  this.classList.remove("clicked");
});


</script>
<head>
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css">
  <link rel="stylesheet" href="https://demo.voidcoders.com/htmldemo/fitgear/main-files/assets/css/animate.css">
<link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.6.3/css/all.css">
<script src="https://code.jquery.com/jquery-2.1.0.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js"></script>
</head>
<body>
    <section class="faq">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-xl-8 col-lg-8 text-center">
                    <div class="section-title">
                        <h4>FAQ's</h4>
                        <h2>Frequently Asking <span>Question’s</span></h2>
                    </div>
                </div>
            </div>
    
            <div class="row">
                <div class="col-xl-12 col-lg-12">
                    <div class="accordion" id="accordionExample">
                        <div class="row">
                            <div class="col-xl-6 col-lg-6">
                                <div class="card">
                                    <div class="card-header">
                                        <h5 class="mb-0">
                                            <button class="btn btn-link collapsed" type="button" data-toggle="collapse"
                                                data-target="#collapseOne" aria-expanded="false" aria-controls="collapseOne">
                                                What is Lorem Ipsum?
                                            </button>
                                        </h5>
                                    </div>
    
                                    <div id="collapseOne" class="collapse" data-parent="#accordionExample">
                                        <div class="card-body">
                                            Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer.
                                        </div>
                                    </div>
                                </div>
    
                                <div class="card">
                                    <div class="card-header">
                                        <h5 class="mb-0">
                                            <button class="btn btn-link collapsed" type="button" data-toggle="collapse"
                                                data-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
                                                Where does it come from?
                                            </button>
                                        </h5>
                                    </div>
                                    <div id="collapseTwo" class="collapse" data-parent="#accordionExample">
                                        <div class="card-body">
                                            Contrary to popular belief, Lorem Ipsum is not simply random text. It has roots in a piece of classical Latin literature from 45 BC, making it over 2000 years old. 
                                        </div>
                                    </div>
                                </div>
    
                                <div class="card">
                                    <div class="card-header">
                                        <h5 class="mb-0">
                                            <button class="btn btn-link collapsed" type="button" data-toggle="collapse"
                                                data-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
                                               Why do we use it?
                                            </button>
                                        </h5>
                                    </div>
                                    <div id="collapseThree" class="collapse" data-parent="#accordionExample">
                                        <div class="card-body">
                                            It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. 
                                        </div>
                                    </div>
                                </div>
    
                                <div class="card">
                                    <div class="card-header">
                                        <h5 class="mb-0">
                                            <button class="btn btn-link collapsed" type="button" data-toggle="collapse"
                                                data-target="#collapse4" aria-expanded="false" aria-controls="collapseThree">
                                                Where can I get some?
                                            </button>
                                        </h5>
                                    </div>
                                    <div id="collapse4" class="collapse" data-parent="#accordionExample">
                                        <div class="card-body">
                                            There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour
                                        </div>
                                    </div>
                                </div>
                            </div>
    
                            <div class="col-xl-6 col-lg-6">
                                <div class="card">
                                    <div class="card-header">
                                        <h5 class="mb-0">
                                            <button class="btn btn-link collapsed" type="button" data-toggle="collapse"
                                                data-target="#collapse5" aria-expanded="false" aria-controls="collapseOne">
                                                What is Lorem Ipsum?
                                            </button>
                                        </h5>
                                    </div>
    
                                    <div id="collapse5" class="collapse" data-parent="#accordionExample">
                                        <div class="card-body">
                                            Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer.
                                        </div>
                                    </div>
                                </div>
    
                                <div class="card">
                                    <div class="card-header">
                                        <h5 class="mb-0">
                                            <button class="btn btn-link collapsed" type="button" data-toggle="collapse"
                                                data-target="#collapse6" aria-expanded="false" aria-controls="collapseTwo">
                                                Where does it come from?
                                            </button>
                                        </h5>
                                    </div>
                                    <div id="collapse6" class="collapse" data-parent="#accordionExample">
                                        <div class="card-body">
                                            Contrary to popular belief, Lorem Ipsum is not simply random text. It has roots in a piece of classical Latin literature from 45 BC, making it over 2000 years old. 
                                        </div>
                                    </div>
                                </div>
    
                                <div class="card">
                                    <div class="card-header">
                                        <h5 class="mb-0">
                                            <button class="btn btn-link collapsed" type="button" data-toggle="collapse"
                                                data-target="#collapse7" aria-expanded="false" aria-controls="collapseThree">
                                                Why do we use it?
                                            </button>
                                        </h5>
                                    </div>
                                    <div id="collapse7" class="collapse" data-parent="#accordionExample">
                                        <div class="card-body">
                                            It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout.
                                        </div>
                                    </div>
                                </div>
                                <div class="card">
                                    <div class="card-header">
                                        <h5 class="mb-0">
                                            <button class="btn btn-link collapsed" type="button" data-toggle="collapse"
                                                data-target="#collapse8" aria-expanded="false" aria-controls="collapseThree">
                                                Where can I get some?
                                            </button>
                                        </h5>
                                    </div>
                                    <div id="collapse8" class="collapse" data-parent="#accordionExample">
                                        <div class="card-body">
                                            
                                            There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour
                                        </div>
                                    </div>
                                </div>
    
                            </div>
    
                        </div>
    
                    </div>
    
                </div>
            </div>
        </div>
    </section>


</body>
<style>
   h1, h2, h3, h4, h5, h6 {
    color: #ff008b;
}
section {
    padding: 60px;
}
a, a:hover, a:focus, a:active {
    text-decoration: none;
    outline: none;
}
ul {
    margin: 0;
    padding: 0;
    list-style: none;
}
.faq {
    padding: 120px 0 90px;
    min-height: 100vh;
}

.faq .section-title {
    margin-bottom: 54px;
}

.faq .section-title h2 {
    margin-bottom: 22px;
}

.faq .accordion .card {
    border: none;
    margin-bottom: 30px;
}

.faq .accordion .card:not(:first-of-type) .card-header:first-child {
    border-radius: 10px;
}

.faq .accordion .card .card-header {
    border: none;
    border-radius: 10px;
    padding: 0;
}

.faq .accordion .card .card-header h5 {
    padding: 0;
}

.faq .accordion .card .card-header h5 button {
    color: #1e3056;
    font-size: 18px;
    font-weight: 500;
    text-decoration: none;
    padding: 0 30px 0 70px;
    height: 80px;
    display: block;
    width: 100%;
    color: rgba(0, 0, 0, 0.8);
    text-align: left;
    background: rgb(255, 255, 255);
    -webkit-box-shadow: 0px -50px 140px 0px rgba(69, 81, 100, 0.1);
    box-shadow: 0px -50px 140px 0px rgba(69, 81, 100, 0.1);
    border-radius: 10px 10px 0 0;
    position: relative;
}

.faq .accordion .card .card-header h5 button:after {
    position: absolute;
    left: 30px;
    top: 50%;
    margin-top: -10px;
    width: 20px;
    height: 20px;
    background-color: transparent;
    color: #ff5f74;
    text-align: center;
    border: 1px solid #ff5f74;
    border-radius: 50%;
    line-height: 100%;
    content: '\f067';
    font-size: 10px;
    line-height: 18px;
    font-family: "Font Awesome 5 Free";
    font-weight: 900;
}

.faq .accordion .card .card-header h5 button.collapsed {
    background: #000000e0;
    color: white;
    -webkit-box-shadow: none;
    box-shadow: none;
}

.faq .accordion .card .card-header h5 button[aria-expanded="true"]:after {
    content: '\f068';
    color: rgb(190, 56, 56);
    background-image: -webkit-linear-gradient(-180deg, #5e7eff 0%, #ff5f74 30%, #a85fff 100%);
}

.faq .accordion .card .card-body {
    -webkit-box-shadow: 0px 15px 140px 0px rgba(69, 81, 100, 0.1);
    box-shadow: 0px 15px 140px 0px rgba(69, 81, 100, 0.1);
    border-radius: 0 0 10px 10px;
    padding-top: 0;
    margin-top: -6px;
    padding-left: 72px;
    padding-right: 70px;
    padding-bottom: 23px;
    color: rgba(30, 48, 86, 0.8);
    line-height: 30px;
}
</style>