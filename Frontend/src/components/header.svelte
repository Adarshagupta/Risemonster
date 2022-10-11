<body>
    <aside>

    </aside>
    <input type="checkbox" id="menu-toggle"/>
      <label id="trigger" for="menu-toggle"></label>
      <label id="burger" for="menu-toggle"></label>
      <ul id="menu">
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Portfolio</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
</body>
<style>
    
    @import url(https://fonts.googleapis.com/css?family=Roboto:400,700);

    @keyframes checked-anim {
        10% {
            width: 10px;
            height: 10px;
        }
        20% {
            width: 100px;
            height: 100px;
        }

    50% {
        width: 200px;
        height: 200px;
    }
    75%{
        width: 210px;
        height: 210px;
    }
    100% {
        width: 40%;
        height: 50%;
        border-radius: 0;
    }
}
@keyframes not-checked-anim {
    0% {
        width: 50px;
        height: 50px;
    }
}li, a {
    margin: 75px 0 -55px 0;
    color: #d9dd00;
    font: 14pt "Roboto", sans-serif;
    font-weight: 700;
    line-height: 1.8;
    text-decoration: none;
    text-transform: none;
    list-style: none;
    outline: 0;
    display: none;
    top: 0;
    lefrightt: 0;
}
li {
    width: 230px;
    text-indent: 56px;}

aside {
    position: absolute;
    color: rgb(0, 0, 0);
    top: 35%;
    right: 10%;
    text-align: right;
}
h1 {
    line-height: 0;
    font-size: 4vw;
    font-weight: 700;
}
h3 {
    float: right;
    line-height: .3;
    font-size: 2.5vw;
    font-weight: lighter;
}
h4 {
    float: left;
    margin-left: -2%;
    font-size: 1.5vw;
    font-weight: lighter;
}

html, body {
    
    background-color: #03A9F4;
    font-family: 'Roboto', sans-serif;
    overflow: hidden;
}

#trigger, #burger, #burger:before, #burger:after {
    position: absolute;
    top: 40px;
    right: 10%;
    background: #fbff00;
    width: 30px;
    height: 5px;
    transition: .2s ease;
    cursor: pointer;
    z-index: 1;
}
#trigger {
    height: 25px;
    background: none;
}
#burger:before {
    content: " ";
    top: 10px;
    right: 0;
}
#burger:after {
    content: " ";
    top: 20px;
    right: 0;
}
#menu-toggle:checked + #trigger + #burger {
    transform: rotate(180deg);
    transition: transform .2s ease;
}

#menu-toggle:checked + #trigger + #burger:before {
    width: 20px;
    top: -2px;
    right: 18px;
    transform: rotate(45deg) translateX(-5px);
    transition: transform .2s ease;
}
#menu-toggle:checked + #trigger + #burger:after {
    width: 20px;
    top: 2px;
    right: 18px;
    transform: rotate(-45deg) translateX(-5px);
    transition: transform .0s ease;
}
#menu {
    position: absolute;
    margin: 0; padding: 0;
right: 0;
    background-color: rgb(0, 0, 0);
    border-bottom-right-radius: 100%;
    box-shadow: 0 2px 5px rgba(0,0,0,0.26);
    animation: not-checked-anim -5s both;
    transition: -5s;
    border-radius: 10px;
}
#menu-toggle:checked + #trigger + #burger + #menu {
    animation: checked-anim 1s ease both;
}
#menu-toggle:checked + #trigger ~ #menu > li, a {
    display: block;
}
[type="checkbox"]:not(:checked), [type="checkbox"]:checked {
    display: none;
}
</style>