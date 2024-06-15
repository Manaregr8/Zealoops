<script>import cycle from "../new-assets/images/cycleze1/3.png";
import cycle2 from "../new-assets/images/cycleze2/5.png";
import cycle3 from "../new-assets/images/cycleeco/2.png";
  import banner from "../new-assets/images/banner.jpg";
  import arrow from "../new-assets/icons/arrow.png";
  import amazon from "../new-assets/icons/social.png";
  import Flipkart from "../new-assets/icons/pngwing.com.png";
  import Whatsaap from "../new-assets/icons/whatsapp.png";
  import { lazyLoad } from './lazyLoad.js';
  let showBuyOptions = false;
  let shoBuyOptions = false;
  let shBuyOptions = false;

const toggleBuyOptions = () => {
  showBuyOptions = !showBuyOptions;
};

const closeBuyOptions = () => {
  showBuyOptions = false;
};


const togglBuyOptions = () => {
  shoBuyOptions = !shoBuyOptions;
};

const closBuyOptions = () => {
  shoBuyOptions = false;
};
const toggBuyOptions = () => {
  shBuyOptions = !showBuyOptions;
};

const cloBuyOptions = () => {
  shBuyOptions = false;
};
  </script>
	<h1>Our <span style="color: #FDAF35;">Products</span></h1>
<section >
  <div class="grid" style="background-image:url({banner})">
    <div class="text">
      <h4>Ze <span style="color: #FDAF35;">1</span></h4>
      <h2>TAKE ON THE CITY WITH
        <span style="color: #FDAF35;">CONFIDENCE</span></h2>

      
      <p style="color: #FDAF35;">Ride away with upto 20% Discount</p>
      <div class="modes">
      <p>Available in 2 modes: </p>
      <div class="buttonsection">
      <button>Manual</button><button>Electric</button></div></div>
      <button on:click={toggleBuyOptions}>Buy Now</button>
    </div>
    <img use:lazyLoad={cycle} alt="ProductImage">
  </div> 
</section>
{#if showBuyOptions}
<div class="display" id="onBuy">
<div class="card">
  <a href="#" on:click|preventDefault={closeBuyOptions}><p>X-CLOSE-X</p></a>
  <a href="https://www.amazon.in/Zealoops-Electric-Non-Removable-Battery-Suspension/dp/B0CR44VCMB"><img use:lazyLoad={amazon} alt=""><p>Amazon : Buy from Amazon</p></a>
  <a href="#" disable><img use:lazyLoad={Flipkart} alt=""><p>Flipkart : Buy from Flipkart (coming soon)</p></a>
  <a href="https://api.whatsapp.com/send?phone=+919105300803&text=%C2%A0"><img use:lazyLoad={Whatsaap} alt=""><p>Whatsaap : Buy from Us</p></a>
</div>
</div>
{/if}
<section >
  <div class="grid" style="background-image:url({banner})">
    <div class="text">
      <h4>Ze <span style="color: #FDAF35;">2</span></h4>
      <h2>TAKE ON THE CITY WITH
        <span style="color: #FDAF35;">CONFIDENCE</span></h2>

      
      <p style="color: #FDAF35;">Ride away with upto 20% Discount</p>
      <div class="modes">

        <p>Available in 2 modes: </p>
        <div class="buttonsection">
        <button>Manual</button><button>Electric</button></div></div>
       <button on:click={togglBuyOptions}>Buy Now</button>
    </div>
    <img src={cycle2} alt="ProductImage">
  </div> 
</section>
{#if shoBuyOptions}
<div class="display" id="onBuy">
<div class="card">
  <a href="#" on:click|preventDefault={closBuyOptions}><p>X-CLOSE-X</p></a>
  <a href="https://www.amazon.in/Zealoops-Electric-Non-Removable-Battery-Suspension/dp/B0CR3HKN9M/ref=sr_1_1?crid=2E7LF6H0G5K5K&dib=eyJ2IjoiMSJ9.hUGGNn5rDxQ-T3H0vY7AUQ.GVyu6IKL9p9wiSD_tfZmU5Aq9KHx4QlPmMMBWWCcH_I&dib_tag=se&keywords=zealoops&qid=1710296076&sprefix=zealoo%2Caps%2C375&sr=8-1"><img src={amazon} alt=""><p>Amazon : Buy from Amazon</p></a>
  <a href="#" disable><img src={Flipkart} alt=""><p>Flipkart : Buy from Flipkart (coming soon)</p></a>
  <a href="https://api.whatsapp.com/send?phone=+919105300803&text=%C2%A0"><img src={Whatsaap} alt=""><p>Whatsaap : Buy from Us</p></a>
</div>
</div>
{/if}
<section >
  <div class="grid" style="background-image:url({banner})">
    <div class="text">
      <h4>Ze <span style="color: #FDAF35;">eco</span></h4>
      <h2>TAKE ON THE CITY WITH
        <span style="color: #FDAF35;">CONFIDENCE</span></h2>

      
      <p style="color: #FDAF35;">Ride away with upto 20% Discount</p>
      <div class="modes">

        <p>Available in 2 modes: </p>
        <div class="buttonsection">
        <button>Manual</button><button>Electric</button></div></div>
        <button on:click={toggBuyOptions}>Buy Now</button>
    </div>
    <img src={cycle3} alt="ProductImage">
  </div> 
</section>
{#if shBuyOptions}
<div class="display" id="onBuy">
<div class="card">
  <a href="#" on:click|preventDefault={cloBuyOptions}><p>X-CLOSE-X</p></a>
  <a href="#"><img src={amazon} alt=""><p>Amazon : Buy from Amazon (coming soon)</p></a>
  <a href="#" disable><img src={Flipkart} alt=""><p>Flipkart : Buy from Flipkart (coming soon)</p></a>
  <a href="https://api.whatsapp.com/send?phone=+919105300803&text=%C2%A0"><img src={Whatsaap} alt=""><p>Whatsaap : Buy from Us</p></a>
</div>
</div>
{/if}
<style>
    section{
        width: 100%;
        max-width: 1300px;
        box-sizing: border-box;
        margin: 10px auto 10px auto;
        color: white;
        box-sizing: border-box;
    }
    .display{
      height: 100vh;
      width: 100%;
      position: absolute;
      z-index: 1000000;
      background-color: rgba(0, 0, 0, 0.314);
      top: 0;
      left: 0;
      position: fixed;
      display: flex;
      justify-content: center;
      align-items: center;
      box-sizing: border-box;
    }
    .card{
      background-color: white;
      border-radius: 10px;
      padding: 10px;
      display: flex;
      flex-direction: column;
      width: 100%;
      max-width: 300px;

    }
    .card a{
      display: flex;
      padding: 10px 15px;
      align-items: center;
      width: 100%;
      
    }
    a p{
      font-size: 16px;
    }
    .card img{
     width: 100%;
     max-width: 40px;
      padding-right: 10px;
    }
    .grid{
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-gap:20px;
        border: 1px solid #75758A;
        border-radius: 10px;
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        margin: 10px 16px;
        padding: 20px 40px 20px 40px;
        font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    }
    h4{
      font-size: 40px;
      font-family: 'Space Age', sans-serif;
      font-weight: 200;
      padding: 10px 0;
    }
    p{
      font-family: Raleway;
      font-weight: 100;
    }
    h2{
      font-family: Raleway;
      font-weight: 900;
      font-size: 30px;
    }
    .modes{
      padding: 10px 0;
      display: grid;
      grid-template-columns: 1fr;
    }
    .modes button{
      padding: 5px 10px;
      margin: 0 5px 0 0;
      border: none;
      background-color: #FDAF35;
      border-radius: 2px;
      color:white;
      font-size: 16px;
      font-weight: 700;
      text-transform: uppercase;
    }
    .text{
      display: flex;
      flex-direction: column;
      justify-content: center;
    }
    button{
      padding: 10px 1px;
      border: none;
      background-color: #FDAF35;
      border-radius: 2px;
      border: none;
      color:white;
      font-weight: 700;
      text-transform: uppercase;
      max-width: 150px;
      margin: 10px 0;
      cursor: pointer;
      font-size: 18.5px;
      text-decoration: none;
    }
    section img{
      width: 100%;
      margin-top: auto;
      max-width: 500px;
    }
   a  img{
      width: 15px;
    }
    .buttonsection{
display: flex;
flex-direction: row;
    }
    .buttonsection button{
      background-color: transparent;
      border-left: 1px solid #FDAF35;
      color: white;
      font-weight: 200;
    }   
    h1{
			font-size: 30px;
			padding:  10px 0 0 16px;
			   font-family: Raleway;
         font-weight: 900;
			   font-size: 30px;
			   text-transform: uppercase;
			   text-align: center;

		}
    @media (max-width:934px){
      .grid{
        padding: 20px;
        grid-template-columns: 0.7fr 1fr;
        grid-gap: 0;
      }
    }
    @media (max-width:832px){
      h4{
      font-size: 30px;
    }
    h2{
      font-size: 25px;
    }
p{
  font-size: 14px;
}
    a{
      font-size: 16px;
    }
    section img{
      width: 100%;
    }
    a img{
      width: 13px;
    }
    .grid{
      padding: 10px;
    }
    }
    @media (max-width:681px){
      h4{
      font-size: 25px;
    }
    h2{
      font-size: 20px;
    }
p{
  font-size: 14px;
}
    a{
      font-size: 15px;
    }
    section img{
      width: 100%;
    }
    .modes button{
      font-size: 15px;
    }
    a img{
      width: 12px;
    }
    .grid{
      padding: 10px;
    }
    }
	    @media (max-width:634px){
    h1{
        font-size: 22px;
    }

    }
    @media (max-width:616px){
      h4{
      font-size: 19px;
      padding: 10px 0 5px 0;
    }
    h2{
      font-size: 18px;
    }
p{
  font-size: 12px;
}
    a{
      font-size: 12px;
    }
    section img{
      width: 100%;
    }
    .modes button{
      font-size: 12px;
    }
    a img{
      width: 11px;
    }
    .modes{
      padding:5px 0;
    }
    button{
      margin: 5px 0 10px 0;
    }
    }
    @media (max-width:524px){
      .modes{
        display: none;
      }
    }
    @media (max-width:421px){
      h4{
      font-size: 14px;
      padding: 10px 0 5px 0;
    }
    h2{
      font-size: 14px;
    }
p{
  font-size: 10px;
}
    a{
      font-size: 12px;
      width: 70px;
    }
    section img{
      width: 100%;
    }
    .modes button{
      font-size: 12px;
    }
    a img{
      width: 11px;
    }
    .modes{
      padding:5px 0;
    }
    a{
      margin: 5px 0 10px 0;
    }
    }
    @media (max-width:394px){
      .grid{
        grid-template-columns: 1fr;
      }
    }
    @media (max-width:370px){
        h1{
            font-size: 22px;
        }
    }
   
 
   
</style>
