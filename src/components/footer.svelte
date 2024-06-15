<script>
    import facebook from "../new-assets/icons/face.png";
    import twitter from "../new-assets/icons/twit.png";
    import linkdin from "../new-assets/icons/linkedin.png";
    import Instagram from "../new-assets/icons/instagram.png"
    import { Link } from 'svelte-routing';
    import { lazyLoad } from './lazyLoad.js';
</script>
<footer>
    <div class="gap"></div>
    <div class="graphic-content">
        <div class="logo-data">
            <h3>Zeal<span style="color:white;">oo</span>ps</h3>
            <p><span style="color:#FDAF35">Back To Basic!</span></p>
            <p>We view art as more than just a product; it's an emotion. Through our frames, we aim to convey an experience of artistry, where each piece becomes a vessel for creativity and expression</p>
            <div class="icon-links">
                <a href="https://www.facebook.com/zealoops?mibextid=JRoKGi"><img use:lazyLoad={facebook} alt="facebook-logo"></a>
                <a href="https://x.com/Zealoops_01?t=LWriSZwMf82N_Ln0mL4NXw&s=08"><img id="twit" use:lazyLoad={twitter} alt="twitter-logo"></a>
                <a href="https://www.linkedin.com/company/zealoops/"><img use:lazyLoad={linkdin} alt="linkdin-logo"></a>
                <a href="https://www.instagram.com/zealoops/"><img use:lazyLoad={Instagram} alt="instagram-logo"></a>
            </div>
        </div>
        <div class="data">
        <div class="sub-data">
            <h4>Quick Links</h4>
            <a href="/"><Link to="/" style="color:#767B88" >Home</Link></a>
            <a href="/about"><Link to="/about" style="color:#767B88" >About</Link></a>
            <a href="/contact"><Link to="/contact" style="color:#767B88" >Contact</Link></a>
        </div>
        <div class="sub-data">
            <h4>Support</h4>
            <a href="/warranty"><Link to="/warranty" style="color:#767B88" >warranty policy</Link></a>
            <a href="/terms"><Link to="/terms" style="color:#767B88" >terms & condition</Link></a>
            <a href="/privacy"><Link to="/privacy" style="color:#767B88" >privacy policy</Link></a>
            <a href="/return"><Link to="/return" style="color:#767B88" >return policy</Link></a>
        </div>
        <div class="sub-data">
            <h4>Also visit us at</h4>
            <a href="https://www.amazon.in/Zealoops-Electric-Non-Removable-Battery-Suspension/dp/B0CR44VCMB"  >amazon</a>
            <a href="https://www.facebook.com/zealoops?mibextid=JRoKGi"  >facebook</a>
            <a href="/"><Link to="/" style="color:#767B88" >Zealoops</Link></a>

        </div>
    </div>
    </div>
</footer>
<style>
      @font-face{
        src: url(../fonts/space-age.regular.ttf);
        font-family: space-age;       
    }
    @font-face{
        src: url(../fonts/Raleway-Medium.ttf);
        font-family: Raleway-Medium;       
    }
    @font-face{
        src: url(../fonts/Raleway-Light.ttf);
        font-family: Raleway-Light;       
    }
    @font-face{
        src: url(../fonts/Raleway-SemiBold.ttf);
        font-family: Raleway-SemiBold;       
    }

    footer{
        width: 100%;
        display: grid;
        grid-template-columns: 100px 1fr;
        color: white;
        font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    }
    .graphic-content{
        display: grid;
        grid-template-columns: 1fr 1fr;
        height: 500px;
        background-color: #1E1D25;
        width: 100%;
        border-top-left-radius: 50px;
    }
    .logo-data{
        display: flex;
        flex-direction: column;
        padding: 0 0 0 40px;
        justify-content: center;
        height: 100%;
    }
    .sub-data{
        display: flex;
        flex-direction: column;
        justify-content: center;
        height: 100%;
    }
    .sub-data a{
        text-decoration: none;
        color: #767B88;
        text-transform: uppercase;
        font-weight: 300;
        padding: 15px 0 0 20px;
        font-family: Raleway;       
    }
    .sub-data a:hover{
        color: #FDAF35;
    }
    footer h3{
        font-family: 'Space Age', sans-serif;
        font-size: 40px;
        font-weight: 400;
        padding: 0 20px;
        color: #FDAF35;
       
    }
    footer p{
        padding: 10px 20px;
        width: 100%;
        max-width: 400px;
        font-family: Raleway;
        font-weight: 100;
    }
    footer h4{
        text-transform: uppercase;
        font-size: 20px;
        font-weight: 700;
        padding: 20px 0 0 20px;
        font-family: Raleway;
        font-weight: 500;
    }
    
    .icon-links{
        width: 100%;

    }
    a img{
        width: 50px;
        padding: 15px 0 0 20px;
    }
    .data{
        display: grid;
        grid-template-columns: 200px 200px 200px;
    }
    @media (max-width:1128px){
        .graphic-content{
        grid-template-columns: 1fr;
    }
    footer h3{
        font-size: 35px;
    }
    .logo-data{
        padding: 0 0 0 0;
    }
    
    }
    @media (max-width:746px){
        .data{
        grid-template-columns:200px 200px;
    }
    .graphic-content{
        height: 100%;
        padding: 20px 0;
    }
    footer h3{
        font-size: 27px;
    }
    }
    @media (max-width:653px){
        footer p{
font-size: 12px;

    }
    }
    @media (max-width:554px){
        .data{
        grid-template-columns:200px;
    }
    .graphic-content{
        height: 100%;
        padding: 20px 0;
    }
    .logo-data{
        width: 100%;
    }
    footer h3{
        font-size: 20px;
        padding: 0 10px;
    }
    footer h4{
        font-size: 16px;
    }
    footer p{
font-size: 12px;
width: 300px;
    }
    .sub-data a{
        font-size: 12px;
        padding: 10px 0 0 10px;
    }
    footer p{
        padding: 0 10px;
    }
    a img{
        width: 35px;
        padding: 10px 0 0 10px;
    }
    footer h4{
        padding: 10px 0 0 10px;
    }
}
    @media (max-width:439px){
        footer p{
font-size: 12px;
width: 250px;
    }
    footer{
        grid-template-columns: 30px 1fr;
    }
    }
    @media(max-width:314px){
        footer p{
            font-size: 10px;
            width: 200px;
        }
        footer h3{
            font-size: 18px;
        }
        footer h4{
            font-size: 12px;
        }
        .sub-data a{
            font-size: 10px;
            padding: 6px 0 0 10px;
        }
    }
</style>