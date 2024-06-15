<script>
    import one from "../new-assets/accesories/2.jpg";
    import two from "../new-assets/accesories/3.jpg";
    import three from "../new-assets/accesories/4.jpg";
    import four from "../new-assets/accesories/5.jpg";
    import five from "../new-assets/accesories/6.jpg";
    import six from "../new-assets/accesories/7.jpg";
    import seven from "../new-assets/accesories/12.jpg";
    import eight from "../new-assets/accesories/9.jpg";
    import nine from "../new-assets/accesories/13.jpg";
    import ten from "../new-assets/accesories/11.jpg";
    import eleven from "../new-assets/accesories/15.jpg";
    import twelve from "../new-assets/accesories/20.jpg";
    import { lazyLoad } from './lazyLoad.js';
</script>
<section>
    <header>
    <h2>Accessories and <span style="color: #FDAF35;">Parts</span></h2>
</header>
    <div class="grid">
        <div class="cards">
            <img use:lazyLoad={one} alt="Alloy-Padels">
            <a href="https://api.whatsapp.com/send?phone=+919105300803&text=I%20Want%20to%20Enquire%20About%20Accesoories">Buy Now</a>
        </div>
        <div class="cards">
            <img use:lazyLoad={two} alt="">
            <a href="https://api.whatsapp.com/send?phone=+919105300803&text=I%20Want%20to%20Enquire%20About%20Accesoories">Buy Now</a>
        </div>
        <div class="cards">
            <img use:lazyLoad={three} alt="">
            <a href="https://api.whatsapp.com/send?phone=+919105300803&text=I%20Want%20to%20Enquire%20About%20Accesoories">Buy Now</a>
        </div>
        <div class="cards">
            <img use:lazyLoad={four} alt="">
            <a href="https://api.whatsapp.com/send?phone=+919105300803&text=I%20Want%20to%20Enquire%20About%20Accesoories">Buy Now</a>
        </div>
        <div class="cards">
            <img use:lazyLoad={five} alt="">
            <a href="https://api.whatsapp.com/send?phone=+919105300803&text=I%20Want%20to%20Enquire%20About%20Accesoories">Buy Now</a>
        </div>
        <div class="cards">
            <img use:lazyLoad={six} alt="">
            <a href="https://api.whatsapp.com/send?phone=+919105300803&text=I%20Want%20to%20Enquire%20About%20Accesoories">Buy Now</a>
        </div>
        <div class="cards">
            <img use:lazyLoad={seven} alt="">
            <a href="https://api.whatsapp.com/send?phone=+919105300803&text=I%20Want%20to%20Enquire%20About%20Accesoories">Buy Now</a>
        </div>
        <div class="cards">
            <img use:lazyLoad={eight} alt="">
            <a href="https://api.whatsapp.com/send?phone=+919105300803&text=I%20Want%20to%20Enquire%20About%20Accesoories">Buy Now</a>
        </div>
        <div class="cards">
            <img use:lazyLoad={nine} alt="">
            <a href="https://api.whatsapp.com/send?phone=+919105300803&text=I%20Want%20to%20Enquire%20About%20Accesoories">Buy Now</a>
        </div>
        <div class="cards">
            <img use:lazyLoad={ten} alt="">
            <a href="https://api.whatsapp.com/send?phone=+919105300803&text=I%20Want%20to%20Enquire%20About%20Accesoories">Buy Now</a>
        </div>
        <div class="cards">
            <img use:lazyLoad={eleven} alt="">
            <a href="https://api.whatsapp.com/send?phone=+919105300803&text=I%20Want%20to%20Enquire%20About%20Accesoories">Buy Now</a>
        </div>
        <div class="cards">
            <img use:lazyLoad={twelve} alt="">
            <a href="https://api.whatsapp.com/send?phone=+919105300803&text=I%20Want%20to%20Enquire%20About%20Accesoories">Buy Now</a>
        </div>
    </div>
</section>
<style>
    section {
        width: 100%;
        margin: auto;
        max-width: 1300px;
        font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
        box-sizing: border-box;
        padding: 16px;
    }
    header{
display: flex;
align-items: center;
    } 
    .cards a{
  color: white;
  font-size: 17px;
  text-decoration: none;
  width: 100%;
  background-color: #1E1D25;
  text-align: center;
  padding: 10px 0;
  margin-top: auto;
    }
    h2 {
        text-transform: uppercase;
        font-size: 40px;
        font-weight: 900;
        font-family: Raleway;
    }
    .grid {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr;
        grid-gap: 10px;
        width: 100%;
        margin: 35px 0;
    }
    p{
        font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
        padding: 5px 10px;
        font-weight: 700;
        color: black;
        margin-top: auto;
    }
    .cards {
        width: 100%;
        max-width: 300px; /* Set max-width to limit card width */

        background-color: white;
        border-radius: 10px;
        border: 1px solid #dedede;
        box-shadow:3px 3px 4px #bfbfbf;
        overflow: hidden;
        display: flex;
        flex-direction: column;
    }
    .cards img{
        width: 100%;
        border-radius: 10px;
    }

    .cards:hover img{
        transform: translateY(-15px);
        transition: transform 0.2s ease-in-out;
    }
    @media (max-width:1127px){
        h2{
            font-size: 25px;
        }
        .grid{
            grid-template-columns: 1fr 1fr 1fr 1fr;
        }
    }
    @media (max-width:780px){
    }
    @media (max-width:703px){
        .grid{
            grid-template-columns: 1fr 1fr 1fr;
        }
        p{
            font-size: 14px;
        }
        .cards a{
            font-size: 14px;
            padding: 5px 0;
        }
    }
    @media (max-width:545px){
        .grid{
            grid-template-columns: 1fr 1fr;
        }
        h2{
            font-size: 21px;
        }
    }
    @media (max-width:437px){
        p{
            font-size: 12px;
        }
        .cards a{
            font-size: 12px;
        }
    }
</style>
