<script>
    import banner from "../new-assets/Zee-banner.jpg";
	import { lazyLoad } from './lazyLoad.js';
</script>

<section>
    <img use:lazyLoad={banner} alt="about banner" />
    <div class="text">
        <div class="grid">
            <div class="floatText">
                <p class="floatrightp">PEDAL ASSIST E-BIKE</p>
                <h2>
                    Our frames are developed and engineered to compete in
                    today’s world.
                </h2>
            </div>
            <p>
                Zealoops is brand of Eltires Private Limited ( An Indian company ) that is revolutionizing the
                cycling industry with its innovative and futuristic designs.
                Their cycles and paddle-assist E-cycles are a perfect blend of
                energy, enthusiasm, strong frames, and ruggedness. They are
                designed to provide a great riding experience to everyone from
                beginners to professional cyclists.<br />

                The company has put a lot of effort into researching the best
                materials for their bikes so that they can offer the highest
                quality products to their customers. With Zealoops Electric
                Cycles, you can be sure that you will get a product with
                superior performance and durability
            </p>
        </div>
        <p>
            Our motive is to transform the world of cycles into well-engineered
            and efficiently designed robust e-bikes that offer good speed and
            effective mileage. We believe in delivering products extending
            functionality with pleasing aesthetics. Hence our products are
            developed keeping in mind the requirements of a wide audience to
            make commuting a fun, safe, and healthy experience. We invite you to
            share with us the exhilarated experience of commuting with Zealoops.
        </p>
    </div>
</section>

<style>
    @font-face {
        src: url(../fonts/Raleway-Medium.ttf);
        font-family: Raleway-Medium;
    }
    @font-face {
        src: url(../fonts/Raleway-Light.ttf);
        font-family: Raleway-Light;
    }
    @font-face {
        src: url(../fonts/Raleway-SemiBold.ttf);
        font-family: Raleway-SemiBold;
    }
    section {
        width: 100%;
        max-width: 1300px;
        margin: auto;
        font-family: "DM Sans", sans-serif;
        color: rgb(124, 124, 124);
    }
    .grid {
        display: grid;
        grid-template-columns: 0.8fr 1fr;
        grid-gap: 20px;
        margin-bottom: 20px;
    }
    .floatText {
        display: flex;
        flex-direction: column;
        padding-left: 10px;
    }
    img {
        aspect-ratio: 13.8/6;
        object-fit: cover;
        width: 100%;
    }
    .text {
        width: 100%;
        margin: 30px 0px;
    }
    p {
        font-size: 1.2rem;
        font-family: Raleway;
        font-weight: 100;
    }
    h2 {
        font-size: 2.5rem;
        color: black;
        font-family: Raleway;
        font-weight: 900;
        text-transform: uppercase;
    }
    p {
        padding: 0 16px;
        text-align: justify;
    }
    .floatrightp {
        padding: 0;
    }
    @media (max-width: 720px) {
        .grid {
            grid-template-columns: 1fr;
            grid-gap: 10px;
        }
        h2 {
            font-size: 28px;
        }
        p {
            font-size: 16px;
        }
        .floatText {
            padding: 16px;
        }
    }
    @media (max-width: 653px) {
        p {
            font-size: 12px;
        }
    }
    @media (max-width: 554px) {
        p {
            font-size: 12px;
        }
        .text {
            margin: 15px 0;
        }
        .grid {
            grid-gap: 0px;
        }
        h2 {
            font-size: 20px;
        }
    }

    @media (max-width: 314px) {
        p {
            font-size: 10px;
        }
    }
</style>
