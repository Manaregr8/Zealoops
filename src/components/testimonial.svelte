<script>
    import quote from "../new-assets/icons/quote.png";
    import { lazyLoad } from './lazyLoad.js';
</script>
<section>
    <h1>Ready To <span style="color: #FDAF35;">book your ride</span></h1>
    <a href="https://api.whatsapp.com/send?phone=+9105300803&text=%C2%A0"class="book">Hell Yeah!</a>
    <h2>OUR TESTIMONIALS</h2>
    <div class="testimonails">
        <div class="second">
<img use:lazyLoad={quote} alt="quote-icon">
            <p class="review">This is a good product at this price range.it is light weight and easy to assemble. the services provided is very good</p>
<p class="name">Manjeet Singh</p>
        </div>
       <p>check out more at <a href="https://www.google.com/search?q=zealoops&rlz=1C1GCEO_enIN879IN879&oq=zea&gs_lcrp=EgZjaHJvbWUqDAgEECMYJxiABBiKBTIGCAAQRRg8MgYIARBFGD0yCAgCEEUYJxg7MgYIAxBFGDkyDAgEECMYJxiABBiKBTIGCAUQRRg8MgYIBhBFGD0yBggHEEUYPNIBCDIzOTNqMGo3qAIAsAIA&sourceid=chrome&ie=UTF-8#lrd=0x390cfbf499345ab9:0x36154fa1a0cc7dca,1,,,,">GOOGLE</a></p>
            </div>   
</section>
<style>
    section{
        width: 100%;
        max-width: 1300px;
        margin: auto;
        box-sizing: border-box;
        text-align: center;
        padding: 20px 10px 0 10px;
        font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    }
    h1{
        font-size: 50px;


        font-family: Raleway;
        font-weight: 900;
        text-transform: uppercase;
        padding: 20px 0 30px 0;
    }
    .book{
        background-color: #FDAF35;
        border: none;
        color: white;
        font-size: 20px;
        font-weight: 700;
        padding: 8px 16px;
        border-radius: 5px;
    }
    a{
        text-decoration: none;
        margin: 20px 0;
    }
    h2{
font-size: 40px;
font-family: Raleway;
font-weight: 900;
        text-transform: uppercase;
        padding: 60px 0 0 0;
    }
    .review{
        font-size: 30px;
        width: 60%;
        margin: auto;
        padding: 15px 0;
    }
    .name{
        font-size: 25px;
        font-weight: 700;
        padding: 10px 0;
    }
img{
    padding: 25px 0;
}
p{
    font-family: Raleway;
    font-weight: 100;
}
.testimonails{
margin: 0px 0px 40px 0;

}
.testimonails a{
    color: #FDAF35;
}

    @media (max-width:1127px){
        h2{
            font-size: 25px;
        }
        .review{
            font-size: 25px;
        }
        h1{
            font-size: 30px;
        }
        p{
            font-size: 16px;
        }
    }
    @media (max-width:780px){
        p{
            font-size: 14px;
        }
        h1{
         padding: 10px 10px 10px 10px;   
        }
    }
    @media (max-width:703px){
p{
            font-size: 13px;
        }
        h2{
            padding-top: 30px;
        }
        img{
            padding: 10px 0;
        }
        .review{
            font-size: 18px;
        }
        .book{
        font-size: 17px;
        padding: 5px 10px;
    }
    }
    @media (max-width:545px){
    
        h2{
            font-size: 21px;
        }
        h1{
            font-size: 24px;
        }
        .review{
            width: 100%;
        }

    }
    @media (max-width:437px){

        p{
            font-size: 10px;
        }
        .review{
            font-size: 16px;
            padding-bottom: 10px;
        }
    }
</style>