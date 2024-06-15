<script>
    let paddles = "Alloy Pedals";
    let brakes = "Dual Disc Brakes";
    let Suspension = "Front-suspension";
    let assist = "pedal-assist & throttle";
    let frame = "Robust Steel Frame";
    let wheel = "26 Inch wheel size with alloy rims";
    let battery = "36V 7.8Ah Battery, Upto 60 kms mileage";
    let Gears = "7-speed-gears";
    import frameicon from "../new-assets/icons/Rebust-steel-frame.png";
    import wheelicon from "../new-assets/icons/26-inch-wheel.png";
    import batteryicon from "../new-assets/icons/36V-5-battery-milage.png";
    import gearsicon from "../new-assets/icons/7-speed-gear.png";
    import paddlesicon from "../new-assets/icons/Alloy-pedals.png";
    import brakesicon from "../new-assets/icons/Dual-disc-Breaker.png";
    import Suspensionicon from "../new-assets/icons/Front-suspension.png";
    import assisticon from "../new-assets/icons/pedal-assist-and-throttle.png";
    import { lazyLoad } from './lazyLoad.js';
</script>

<section>
    <div class="grid">
        <div class="flex">
            <h3>Product <span style="color: #FDAF35;">Specifications</span></h3>
        </div>

        <div class="flex-1">
            <div class="grid1">
                <li>
                    <img use:lazyLoad={frameicon} alt="" />
                    <p>{frame}</p>
                </li>
                <li>
                    <img use:lazyLoad={wheelicon} alt="" />
                    <p>{wheel}</p>
                </li>
                <li>
                    <img use:lazyLoad={batteryicon} alt="" />
                    <p>{battery}</p>
                </li>
                <li>
                    <img use:lazyLoad={gearsicon} alt="" />
                    <p>{Gears}</p>
                </li>
            </div>
            <div class="grid2">
                <li>
                    <img use:lazyLoad={paddlesicon} alt="" />
                    <p>{paddles}</p>
                </li>
                <li>
                    <img use:lazyLoad={brakesicon} alt="" />
                    <p>{brakes}</p>
                </li>
                <li>
                    <img use:lazyLoad={Suspensionicon} alt="" />
                    <p>{Suspension}</p>
                </li>
                <li>
                    <img use:lazyLoad={assisticon} alt="" />
                    <p>{assist}</p>
                </li>
            </div>
        </div>
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
        padding: 30px 0;
        width: 100%;
        max-width: 1300px;
        margin: auto;
        text-transform: uppercase;
        box-sizing: border-box;
    }
    .grid {
        display: flex;
        flex-direction: column;
        width: 100%;
    }
    .flex {
        width: 100%;
    }
    .flex-1 {
        width: 100%;
        display: grid;
        grid-template-columns: 1fr 1fr;
    }
    .grid1 {
        padding: 0 10px 0 16px;
    }
    .grid2 {
        padding: 0 16px 0 10px;
    }
    p {
        padding: 0 0 0 15px;
        font-weight: 100;
        font-size: 15px;
        font-family: Raleway;
    }
    h3 {
        padding: 0 0 15px 16px;
        font-size: 35px;
        font-family: Raleway;
        font-weight: 900;
    }
    li {
        display: flex;
        align-items: center;
        padding: 12px 0;
    }
    @media (max-width: 634px) {
        h3 {
            font-size: 25px;
        }
       
        p {
            font-size: 12px;
        }
        li img {
            width: 30px;
        }
        section {
            padding: 20px 0;
        }
        h3 {
            font-size: 20px;
        }
    }
    @media (max-width: 370px) {
        p {
            font-size: 10px;
        }
        li img {
            width: 25px;
        }
        h3 {
            font-size: 17px;
        }
        section {
            padding: 15px 0;
        }
    }
</style>
