<script>
    import Banner from "../new-assets/images/specs.png"
    import { lazyLoad } from './lazyLoad.js';
</script>
<section>
    <div class="grid1">
<span class="big">
    ZEALOOPS
</span>
    </div>
    <div class="grid2">
        <div class="graphic"></div>
        <p>hello</p>
    </div>
    <img use:lazyLoad={Banner} alt="specs">
</section>
<style>
    section{
        width: 100%;
        display: flex;
        flex-direction: column;
        box-sizing: border-box;
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    }
    .big{
        color: #f4f4f4;
        font-size: 150px;
        font-family: 'Space Age', sans-serif;
        text-align: center;

}
.grid1{
    width: 100%;
    max-width:1300px;
    margin: auto;
    text-align: center;
}
.grid2{
    height: 400px;
    max-width: 1300px;
    width:100%;
    margin: auto;
    display: grid;
    grid-template-columns: 1fr 300px;
    padding: 100px 0 0 0;
}
.graphic{
   width:100%;
   height: 100%;
   background-color: #1E1D25;
   border-bottom-left-radius: 50px;
   margin: 0 0 0 10px;
}
.grid2 p{
    display:none;
}
img{
    position: absolute;
    width:100%;
    left: 50%;
    transform: translateX(-50%);
    max-width: 1300px;
}
@media (max-width:1300px){
    .big{
        font-size: 13vw;
        padding-bottom:20px;
    }
}
@media (max-width:1250px){
    .grid2{
    grid-template-columns: 1fr 200px;
    padding: 80px 0 0 0;
}
}
@media (max-width:1127px){
    .grid2{
    grid-template-columns: 1fr 100px;
    padding: 40px 0 0 0;
}
}
@media (max-width:1000px){
    .grid2{
    grid-template-columns: 1fr 100px;
    padding: 0px 0 0 0;
}
}
@media (max-width:940px){
    .grid2{
        height: 100%;
        aspect-ratio: 2.5/1;
}
}
</style>