<script>
    import ServiceBtn from './ServiceBtn.svelte'
    export let heroImage="/assets/images/heros/hmhero1.jpg";
    export let heroTitle="Ultimate Plumbing Supply";
    export let heroBigText="Affordable & High Quality Plumbing Parts & Tools";
    export let heroText="Same Day Delivery Available!";
</script>
<style>
    img {
        max-width: none;
    }
    #hero-section{
        position:relative;
        overflow:hidden;
        background-color:var(--primary-color);
        padding: 5rem 2rem;

    }
    #hero-section .grid-container{
        display:grid;
        grid-template-columns:100%;
    }
    .hero-left{
        position:relative;
        text-align:left;
        height:100%;
        z-index:3;
        background-color:var(--primary-color);
        display:flex;
        flex-direction:column;
        justify-content:center;
        align-items:center;
        align-content:center;
    }
    .hero-right{
        display:none;
        position:relative;
        height:100%;
        margin:0;
        padding:0;
        z-index:1;
    }
    .slant-box{
        position:absolute;
        background-color:var(--primary-color);
        border: none;
        z-index:2;
        top:0;
        left:23.5%;
        margin:0;
        padding:0;
        transform: skewX(-30deg);
        width:100%;
        height:100%;
    }
    .white-hr{
        background: #ffffff;
        position: relative;
        z-index: 14;
        width: 100%;
        margin-top: 0.5rem;
        margin-bottom: 0.5rem;
    }
    .twenty-four-seven{
        position:absolute;
        right:20px;
        bottom:15%;
    }
    .hero-title, .hero-big-text, .hero-text, .hero-link{
        position:relative;
        z-index:3;
        color:white;
        text-align:left;
    }
    .hero-title{
        font-size:25px;
        font-weight:300;
        text-transform: uppercase;
        width: 100%;
    }
    .hero-big-text{
        font-size:35px;
        font-weight:700;
        text-transform: none;

    }
    .hero-text{
        align-self:flex-start;
        font-size:18px;
    }
    .slotted-content{
        position:relative;
        z-index:3;
        align-self:flex-start;

        color:white;
    }
    @media screen and (min-width: 768px){
        #hero-section{
            padding: 0;
        }
        #hero-section .grid-container{
            grid-template-columns: 50% 50%;
        }
        .hero-right{
            display:block;
        }
        .slant-box{
            left:37.5%;
        }
    }
    @media screen and (min-width: 1200px){
        .slant-box{
            left:23.5%;
        }
        .twenty-four-seven{
            right:20px;
            bottom:8%;
        }
        .hero-title{
            font-size:25px;
        }
        .hero-big-text{
            font-size:35px;
        }
    }
    .service-btns-bg{
        background: rgb(61,84,103);
        background: linear-gradient(90deg, rgba(61,84,103,1) 9%, rgba(96,115,130,1) 90%);
    }
    .service-buttons{
        display:grid;
        grid-template-rows:1fr 1fr 1fr;
    }
    @media screen and (min-width:768px){
        .service-btns-bg{
            background: #856e38;
        }
        .service-buttons{
            grid-template-rows:1fr;
            grid-template-columns: 1fr 1fr 1fr;
            max-width: 1140px;
            margin:auto;
        }
    }
</style>
<section id="hero-section">
    <div class="grid-container container">
        <div class="hero-left">
            <hr class="slant-box">
            <h1 class="hero-title">{ heroTitle } <br>
                <span class="hero-big-text">{ heroBigText }</span>
            </h1>
            <hr class="white-hr">
            <p class="hero-text">{ heroText }</p>
            <div class="slotted-content">
                <slot></slot>
            </div>
        </div>
        <div class="hero-right">
            <img src='{heroImage}' alt="{heroTitle}" />
        </div>
    </div>
</section>
<div class="service-btns-bg">
    <section class="service-buttons">
        <ServiceBtn serviceBtnBg="#856e38" serviceLink="/plumbing-pumps" serviceTitle="Sump pumps, ejector pumps, All Kinds Of Pumps" serviceIcon="/assets/images/icons/gear.png" serviceIconAlt="Hvac a/c furnace Repairs Icon">Plumbing Pumps</ServiceBtn>
        <ServiceBtn serviceBtnBg="#856e38" serviceLink="/plumbing-fixtures" serviceTitle="Check Out Our Plumbing Fixtures Here" serviceIcon="/assets/images/icons/money.png" serviceIconAlt="Hvac a/c furnace Replacements Icon">Plumbing Fixtures</ServiceBtn>
        <ServiceBtn serviceBtnBg="#856e38"  serviceLink="/water-heaters" serviceTitle="Only The Best Water Heaters" serviceIcon="/assets/images/icons/calendar.png" serviceIconAlt="Hvac a/c furnace Maintenance Icon">Water Heaters</ServiceBtn>
    </section>
</div>
