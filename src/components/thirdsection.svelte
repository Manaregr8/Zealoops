<script>
    import Frame1 from "../new-assets/images/Frame1.png";
    import { lazyLoad } from './lazyLoad.js';
</script>

<section>
    <div class="grid">
        
        <div class="grid1">
            <h3>
                <span style="color: #FDAF35;">Hand crafted</span> frames
            </h3>
            <p>
                In our workshop, every frame undergoes meticulous handcrafting, infused with passion and dedication. We view art as more than just a product; it's an emotion. Through our frames, we aim to convey an experience of artistry, where each piece becomes a vessel for creativity and expression. Our frames aren't just accessories; they're conduits through which art can be truly felt and appreciated. They embody perfection and serve as a testament to our commitment to excellence. Welcome to our world of meticulously crafted frames, where each piece tells a story of dedication, passion, and the transformative power of art.
            </p>
        </div>
        <div class="grid2">
            <img use:lazyLoad={Frame1} alt="" />
        </div>
    </div>
</section>

<style>
section{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    max-width: 1300px;
    margin: 30px auto;
    background-color: white;
    font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    box-sizing: border-box;
    text-align: right;
}
img{
    width: 100% ;
}
.grid{
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-gap: 20px;
    }
    h3{
        font-size: 40px;
        font-weight: 700;
        text-transform: uppercase;
        color: #1E1D25;
        margin-bottom: 10px ;
        font-family: Raleway;
        font-weight: 900;
    }
    .grid1{
        margin: 10px 16px;
    }
    p{
        color: #484849;
        font-family: Raleway;
        font-weight: 100;
        margin-bottom: 10px;
    }
    p{
        text-align: right;
        margin-bottom: 10px;
    }
    @media (max-width:1127px){
        h3{
            font-size: 25px;
        }
        p{
            font-size: 16px;
        }
        .grid{
    grid-template-columns: 0.8fr 1fr;
    }
    }
    @media (max-width:780px){
        .grid{
            grid-template-columns: 0.7fr 1fr;
            grid-gap: 10px;
        }

        p{
            font-size: 14px;
        }
        section{
            margin: 15px auto;
        }

    }
    @media (max-width:703px){
        section{
            margin: 0 auto;
        }
        .grid{
            grid-template-columns:1fr    ;
        }
        .grid{
           display: flex;
           flex-direction: column-reverse;
        }
        p
        {
            font-size: 13px;
            text-align: justify;
        }

    div p{
        font-size: 13px;
    }
    }
    @media (max-width:545px){
        section{
            margin: 0 auto;
        }
        .grid{
           display: flex;
           flex-direction: column-reverse;
        }
        h3{
            font-size: 21px;
        }

    }
    @media (max-width:437px){

        p{
            font-size: 10px;
            padding-bottom: 10px;
        }
    div p{
        font-size: 10px;
    }
    }
</style>
