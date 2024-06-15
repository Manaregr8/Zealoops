<script>

</script>
<section>
    <div class="grid">
        <iframe src="https://www.youtube.com/embed/tj8yGbtMyL8?si=EN8lWFmTo2_K0JVF?&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
        <div class="data">
            <h3>Its Available in <span style="color: #FDAF35;">5 premium colors</span></h3>
            <p class="p-data">The weather and nature is calling for you to come out. Let's go out for some fresh air. And what better way to do that than on a bicycle? A bicycle in your favourite colour that makes you happy as Spring.<br>
                 The new stylish Zealoops e-cycle are available in 5 vibrant shade options:</p>
            <div class="color-segment">
            <div class="color1"><p>Urban Silver</p></div>
            <div class="color2"><p>Maize Marvel</p></div>
            <div class="color3"><p>Teal Harbor</p></div>
            <div class="color4"><p>Caramel Rose</p></div>
            <div class="color5"><p>Midnight Moss</p></div>
        </div>
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
}
.grid{
    display: grid;
    grid-template-columns: 0.8fr 1fr;
    grid-gap: 20px;
    }
    iframe{
        width: 100%;
        height: 350px;
        padding: 10px;
    }
    .data{
        padding: 16px;
    }
    h3{
        font-size: 40px;
        font-weight: 900;
        text-transform: uppercase;
        color: #1E1D25;
        margin-bottom: 10px ;
        font-family: "Raleway";
    }
    .p-data{
        color: #484849;
        font-family: Raleway;
        margin-bottom: 10px;
        font-weight: 100;
    }
    .color1{
        background-color: #ddddddff;
        color: #484849;
    }
    .color2{
        background-color: #fbba14ff;
        color:#484849;
    }
    .color3{
        background-color: #7ab7b8ff;
        color:#484849;
    }
    .color4{
        background-color: #ce9278ff;
        color:#484849;
    }
    .color5{
        background-color: #134a37ff;
        color: white;
    }
    .color-segment{
        margin: 20px 0;
        display: grid;
        grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
        grid-gap: 7px;
        width: 100%;
        height: 50%;
        font-weight: 700;
    }
    .color-segment div{
        display: flex;
        justify-content: center;
        align-items: center;
        width: 100%;
        max-width: 100px;
        border-radius: 15px;
        height: 200px;
        box-shadow:6px 6px 8px grey;
    }
    .color-segment p{
        transform: rotate(270deg);
        text-transform: uppercase;
    }
    p{
        text-align: justify;
        margin-bottom: 10px;
    }
    @media (max-width:1127px){
        h3{
            font-size: 25px;
        }
        .p-data{
            font-size: 16px;
        }
        .grid{
    grid-template-columns: 0.8fr 1fr;
    }
    iframe{
        height: 250px;
    }
    }
    @media (max-width:780px){
        .grid{
            grid-template-columns: 0.7fr 1fr;
            grid-gap: 10px;
        }

        .p-data{
            font-size: 14px;
        }
        section{
            margin: 15px auto;
        }

    }
    @media(max-width:721px){
        .grid{
            grid-template-columns: 0.8fr 1fr;
            grid-gap: 5px;
        }
        iframe{
            width: 100%;
        }
        section{
            margin: 15px 0;
            width: 100%;

        }
    }
    @media (max-width:703px){
        section{
            margin: 0 auto;
        }
        .grid{
            grid-template-columns:1fr    ;
        }
        iframe{
            padding: 0;
            height: 100%;
            aspect-ratio: 16/8;
        }
        .p-data{
            font-size: 13px;
        }
        .color-segment{
        margin: 10px 0;
        display: flex;
        justify-content: space-between;
        align-items: flex-start;
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
            grid-template-columns:1fr    ;
        }
        iframe{
            padding: 0;
            height: 100%;
            aspect-ratio: 16/8;
        }
        h3{
            font-size: 21px;
        }

    }
    @media (max-width:437px){

        .p-data{
            font-size: 10px;
            padding-bottom: 10px;
        }
        .color-segment{
        margin: 10px 0;
    }
    .color-segment div{
        height: 150px;
    }
    div p{
        font-size: 10px;
    }
    }
    @media (max-width:290px){

section{
    width: 280px;
    overflow: hidden;
    margin: auto;
}
}
</style>