<script>
    import logo from "../new-assets/images/banner.jpg";
    import cycle from "../new-assets/images/g8.png";
    import cycle2 from "../new-assets/images/g3.png";
    import cycle3 from "../new-assets/images/g2.png";
    import { Link } from 'svelte-routing';
    
</script>

<section class="hero" style="background-image: url({logo});">
    <div class="grid">
        <div class="textBanner">

            <h3>ZeaL<span style="color: #FDAF35;">oo</span>ps</h3>
            <p>Delivering you</p>
            <h2>AMAZING || CREATIVE || COMFORTABLE</h2>
            <a href="/products"><Link to="/product">product</Link></a>

        </div>
        <div class="cycleBanner">
            <img id="animated2" src={cycle2} alt="cycle">
            <img id="animated" src={cycle} alt="cycle">
            <img id="animated2" src={cycle3} alt="cycle">
            <img id="animated" src={cycle} alt="cycle">
            <img id="animated2" src={cycle2} alt="cycle">
        </div>
    </div>
</section>
<style>
     @import url('https://fonts.cdnfonts.com/css/space-age');  
     @font-face{
        src: url(../newFonts/space-age.regular.ttf);
        font-family: space-age;       
    }
    @font-face{
        src: url(../newFonts/Raleway-Medium.ttf);
        font-family: Raleway-Medium;       
    }
    @font-face{
        src: url(../../static/fonts/Raleway-Light.ttf);
        font-family: Raleway-Light;       
    }
    @font-face{
        src: url(../../static/fonts/Raleway-SemiBold.ttf);
        font-family: Raleway-SemiBold;       
    }
    section {
        width: 100%;
        margin: auto;
        background-position: center;    
        background-repeat: no-repeat;
        background-size: cover;
        height: 100vh;
    }
    .grid{
        width: 100%;
        max-width: 1300px;
        height: 100%;
        margin: auto;
        padding: 10px 0;
        display: grid;
        grid-template-columns: 300px 1fr;
        color: white;
    }
    .textBanner{
        width: 100%;
        height: 100%;
        display: flex;
        justify-content: center;
        flex-direction: column;
        font-family:system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    }
    .textBanner h3{
        font-size: 50px;
        font-weight: 400;
        padding-left: 7px;
        font-family: 'Space Age', sans-serif;
    }
    .textBanner P{
        padding: 0 0 0 10px;
        margin: 10px 0 0 0;
        color: #FDAF35;
        font-family: Raleway;
        font-weight: 100;
    }
    .textBanner h2{
        width: 100%;
        padding: 0 0 0 10px;
        font-size: 30px;
        font-family: Raleway;
        font-weight: 900;
    }
    .textBanner a{
        background-color: #FDAF35;
        color: black;
        font-size: 25px;
        padding: 7px 4px;
        margin: 10px;
        border-radius: 5px;
        font-family: 'Space Age', sans-serif;
        font-weight: 300;
        cursor: pointer;
        text-align: center;
        text-decoration: none;
    }
    .textBanner a:hover{
        background-color: rgb(225, 225, 225);
        color: blue;
    }
    img{
        width: 100%;
        max-width: 700px;
        padding: 40px;
        object-fit: contain;
        margin-top: auto;
        margin-left: auto;
    }
    .cycleBanner{
        display:flex;
        width: 100%;
        height: 100%;
        overflow: hidden;
        max-width: 700px;
        margin-left: auto;
        margin-top: auto;
    }
    #animated2{
        transform: translateX(0);
        animation: 20s swipe;
        animation-iteration-count: infinite;
    }
    #animated{
        transform: translateX(0);
        animation: 20s swipe ;
        animation-iteration-count: infinite;
    }
    @keyframes swipe{
        0%{
            transform: translateX(-400%);
        }
        16%{
            transform: translateX(-400%);
        }
        21%{
            transform: translateX(-300%);
        }
        37%{
            transform: translateX(-300%);
        }
        42%{
            transform: translateX(-200%);
        }
        58%{
            transform: translateX(-200%);
        }
        63%{
            transform: translateX(-100%);
        }
        79%{
            transform: translateX(-100%);
        }
        84%{
            transform: translateX(0%);
        }
        100%{
            transform: translateX(0%);
        }
    }
    @media (max-width:1197px){
        .textBanner h3{
        font-size: 35px;
    }
    .textBanner h2{
        font-size: 25px;
    }
    }
    @media (max-width:1052px){
        section {
        height: auto;
        aspect-ratio: 16/6;
        padding: 49px 0 0 0;
    }
    img{
        padding: 0;
        max-width: 450px;
        margin: auto;
        padding: 30px;
    }
    }
    @media (max-width:1033px){
        .textBanner h3{
        font-size: 30px;
        padding: 0 0 0 7px;
    }
    .textBanner h2{
        font-size: 25px;
        padding: 0 0 0 7px;
    }
    .textBanner P{
        padding: 0 0 0 7px;
        margin: 10px 0 0 0;
    }
    .textBanner a{
       margin: 7px 0 0 7px;
    }
    img{
        padding: 50px;
    }
}
    @media (max-width:790px){
        .textBanner h3{
        font-size: 25px;
    }
    .textBanner h2{
        font-size: 20px;
    }
    .textBanner a{
        font-size: 18px;
    }
    .grid{
        grid-template-columns: 250px 1fr;
    }
    img{
        max-width: 600px;
        margin: auto;
        padding: 15px;
    }
    }
    @media (max-width:653px){
        .textBanner h3{
        font-size: 22px;
    }
    .textBanner h2{
        font-size: 18px;
    }
    .textBanner a{
        font-size: 16px;
    }
    .textBanner P{
font-size: 12px;
    }
    .grid{
        grid-template-columns: 200px 1fr;
    }
    }
    @media (max-width:523px){
        .textBanner h3{
        font-size: 15px;
    }
    .textBanner h2{
        font-size: 15px;
    }
    .textBanner a{
        font-size: 15px;
    }
    .grid{
        grid-template-columns: 150px 1fr;
    }
    section {
        aspect-ratio: 16/8;
    }
    }
    @media (max-width:446px){
        .textBanner h3{
        font-size: 12px;
    }
    .textBanner h2{
        font-size: 12px;
    }
    .textBanner a{
        font-size: 11px;
        padding: 3px 4px;
    }
    .grid{
        grid-template-columns: 120px 1fr;
    }
    .textBanner p{
        font-size: 10px;
    }
    img{
        margin: 0;
        padding: 0;
    }
    }
  
</style>
