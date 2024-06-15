<script>
import banner from "../new-assets/images/contact_cover.png";
import address from "../new-assets/icons/marker_3.png";
import number from "../new-assets/icons/phone_3.png";
import email from "../new-assets/icons/link_4.png";
import { lazyLoad } from './lazyLoad.js';
let status = "";
const handleSubmit = async data => {
  status = 'Submitting...'
  const formData = new FormData(data.currentTarget)
  const object = Object.fromEntries(formData);
  const json = JSON.stringify(object);

  const response = await fetch("https://api.web3forms.com/submit", {
      method: "POST",
      headers: {
          "Content-Type": "application/json",
          Accept: "application/json",
      },
      body: json
  });
  const result = await response.json();
  if (result.success) {
      console.log(result);
      status = result.message || "Success"
  }

}
</script>
<section >
    <div>
    <img use:lazyLoad={banner} alt="contact banner">
</div>
<div class="grid"  id="contactForm">
    <div class="form">
        <h3>ENQUIRE <span style="color: #FDAF35;">NOW</span></h3>
        <p>For Pricing and more product Details please fillup the form<br>
            We will contact you soon</p>
    <form on:submit|preventDefault={handleSubmit}>
        <input type="hidden" name="access_key" value="0b4cb085-71a4-4e36-81cc-f383ca61fef0">
        <input type="text" name="name" placeholder=" Name" required/>
        <input type="number" name="number" placeholder=" Number" required/>
        <input type="email" name="email" placeholder=" Email" required />
        <textarea name="message" placeholder=" Details Regarding Enquiry here!" required rows="3"></textarea>
        <input type="submit" />
    </form>
    
    <div>{status}</div>
</div>
<div class="links">
    <h3><span style="color: #FDAF35;">Drop</span> us a line</h3>
    <div class="cards"><a href="https://maps.app.goo.gl/6VYtzV1vuQcaEzNp9"><p>B-143, Second Floor, East Side, Rama Park, Uttam Nagar, New Delhi 110059</p></a><img use:lazyLoad={address} alt="address-icon"></div>
    <div class="cards"><p><a href="tel:+919105300803">+91 9105300803</a><img use:lazyLoad={number} alt="address-icon"></div>
    <div class="cards"><p><a href="mailto:info@zealoops.com">info@zealoops.com</a><br><a href="mailto:sales@zealoops.com">sales@zealoops.com</a></p><img use:lazyLoad={email} alt="email-icon"></div>
</div>
</div>
</section>
<style>
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
    section{
        width: 100%;
        max-width: 1300px;
        margin: auto;
        font-family: "DM Sans", sans-serif;
    }
    div{
padding: 10px;
display: flex;
justify-content: center;
align-items: center;
    }
    img{
        width: 98%;
        object-fit: cover;
        object-position: top;
        object-fit: contain;
    }
    .grid{
        display: grid;
        grid-template-columns: 1fr 1fr;
        padding: 16px;
    }
    .form{
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        width: 100%;
    }
    h3{
        font-family:Raleway;
        font-weight: 900;
        font-size: 30px;
        padding: 10px 0;
        text-transform: uppercase;
    }
    p{
        padding: 0 0 10px 0;
        font-family: Raleway;
        font-weight: 100;
    }
    form{
        display: flex;
        flex-direction: column;

        align-items: flex-start;
        width: 100%;
    }
    input[type=text],input[type=email],input[type=number], textarea{
        border: none;
        background-color: rgb(250, 250, 250);
        padding: 10px 5px;
        width: 100%;
        max-width: 400px;
        margin: 10px 0;
        border: 1px solid grey;

    }
input[type=submit]{
    padding: 7px 17px;
    font-size: 15px;
    border: none;
    background-color:  #FDAF35;
    color: white;
    font-weight: 700;
}
    .grid img{
        width: 20px;
        height: 20px
    }
    .links{
        display: flex;
        flex-direction: column;
        justify-content: flex-start;
        align-items: flex-end;
    }
    .cards{
        display: flex;
        background-color: rgb(250, 250, 250);
        align-items: center;
        padding: 10px;
        border: 2px solid 808080;
        margin: 5px 0;
        border-radius: 10px;
    }
    .cards img{
        background-color: #FDAF35;
        width: 40px;
        border-radius: 10px;
        padding: 10px;
        margin: 0 10px;
    }
    .cards p{
        text-align: right;
    }
    a{
        text-decoration: none;
        color: #75758A;
    }
    @media (max-width:885px){
        input[type=text],input[type=email],input[type=number], textarea{
        max-width: 300px;

    } 
    }
    @media(max-width:749px){
        input[type=text],input[type=email],input[type=number], textarea{
        max-width: 200px;

    } 
    }
    @media(max-width:646px){ 
        h3{
font-size: 25px;
    }
    p{
        font-size: 12px;
    }
    }
    @media (max-width:578px){
.grid{
    grid-template-columns: 1fr;
}
.form{
    padding: 0px;
}
.links{
    padding: 0px;
}
input[type=text],input[type=email],input[type=number], textarea{
        max-width: 400px;
        min-width: 100px;
padding: 10px 0;
    }
    }
    @media (max-width:364px){
        p{
            font-size: 10px;
        }
    }
</style>
