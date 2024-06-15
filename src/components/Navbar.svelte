  <script>
    import logo from "../new-assets/images/logo.png";
    import menuIcon from "../new-assets/icons/menu.png";
import whatsaap from "../new-assets/whatsaap-logo.gif";
import { Link } from 'svelte-routing';
let topPosition = '-150%'; // Initial position

function menus() {
  const menuBar = document.querySelector('.data-menu');
  if (topPosition === '0') {
    topPosition = '-150%';
  } else {
    topPosition = '0';
  }
  menuBar.style.transform = `translateY(${topPosition})`; // Corrected this line
}
</script>
<nav>
    <div class="container-nav">
        <img id="logo" src={logo} alt="logo">
        <img id="menu" on:click={menus} src={menuIcon} alt="menu">
        <div class="data-menu">
            <a href="/"><Link to="/">Home</Link></a>
            <a href="/about"><Link to="/about">about</Link></a>
            <a href="/product"><Link to="/product">product</Link></a>
            <a href="/warranty"><Link to="/warranty">warranty</Link></a>
            <a href="/contact"><Link to="/contact">contact</Link></a>
        </div>
    </div>
</nav>
<a class="absolute" href="https://api.whatsapp.com/send?phone=+919105300803&text=%C2%A0"><img src={whatsaap} alt="whatsaap-icon"></a>
<style> 
nav{
    width: 100%;
    display: flex;
    background-color: white;
    justify-content: center;
    align-items: center;
    padding: 10px 0;
    position: fixed;
    z-index: 10000;
    border-bottom: 1px solid rgb(187, 187, 187);
}
.container-nav{
    width: 100%;
    display: flex;
    max-width: 1300px;
}
.data-menu{
    margin-left: auto;
    display: flex;
    font-family: 'Space Age', sans-serif;
    align-items: center;
}
.data-menu a{
    padding: 0 10px;
    text-decoration: none;
    color: black;
    font-size: 20px;
    font-weight: 400;
}
.data-menu a:hover{
    color: #FDAF35;
}
#logo{
    width: 300px;
    padding: 10px;
}
#menu{
    display: none;
    width: 25px;
}
.absolute{
    width: 50px;
}
.absolute img{
    width: 60px;
    position: absolute;
    bottom: 20px;
    left: 20px;
    position: fixed;
    z-index: 1000000;
}
@media (max-width:1052px){
    .data-menu{
        position: absolute;
        flex-direction: column;
        text-align: center;
        top: 53px;
        width: 100%;
        background-color: white;
        z-index: 10000;
        border-top: 2px solid black;
        border-bottom: 2px solid black;
        transform: translateY(-150%);
        transition: 0.6s transform;
    }
    .data-menu a{
        padding: 5px 0;
    }
    #logo{
    width: 200px;
}
#menu{
    display: block;
    margin-left:auto;
    padding: 0 10px;
}
}
@media (max-width:708px){
    a{
        font-size: 12px;
    }
    .data-menu a{
        font-size: 17px;
    }
}
@media (max-width:419px){
    .data-menu{
        top: 49px;
    }
    .data-menu a{
        padding: 5px 0;
        font-size: 15px;
        font-weight: 200;
    }
    #logo{
    width: 150px;
}
#menu{
width: 20px;
}
}
</style>