<script>
    let lpageNames = [
        "heating-cooling-service",
        "hvac-air-conditioning-repair-installation-services",
        "hvac-furnace-repair-services"
    ];
    let lpageCities = [
        "bristol-il",
        "lisbon-il",
        "millbrook-il",
        "newark-il",
        "norway-il",
        "oswego-il",
        "ottawa-il",
        "plano-il",
        "sandwich-il",
        "sheridan-il",
        "somonauk-il",
        "sugar-grove-il",
        "yorkville-il",
    ];
    let getLinks = ()=>{
        let landingLinksArr=[];
        let newLink = "";
        for(let lpCount = 0; lpCount < lpageNames.length;lpCount++){
            for(let lcCount = 0; lcCount < lpageCities.length;lcCount++){
                newLink = lpageNames[lpCount]+'-'+lpageCities[lcCount];
                if(!landingLinksArr.indexOf(newLink) >= 0){
                    landingLinksArr = [...landingLinksArr,newLink];
                }
            }
        }
        return landingLinksArr;
    };
    let landingLinks = getLinks();
    let landingLinksRand = ()=>{
        let linkArr = [];
        for(let i = 0;i < 6; i++){
            let rng = Math.round(Math.random() * (landingLinks.length - 1));
            let linkRef=landingLinks[rng];
            let linkCityState = linkRef.replace("heating-cooling-service-","").replace("hvac-air-conditioning-repair-installation-services-","").replace("hvac-furnace-repair-services-","");
            let linkCsSplit = linkCityState.split('-');
            let linkS = linkCsSplit[linkCsSplit.length - 1].toUpperCase();
            let linkCity = linkCityState.replace("-"+linkS.toLowerCase(),'').replace("-"," ");
            let linkC = linkCity.substr(0,1).toUpperCase() + linkCity.substr(1,linkCity.length - 1);
            if(linkCsSplit.length > 2){
                linkC = linkCsSplit[0].substr(0,1).toUpperCase() + linkCsSplit[0].substr(1,linkCity.length - 1) +" "+ linkCsSplit[1].substr(0,1).toUpperCase() + linkCsSplit[1].substr(1,linkCity.length - 1);
            }
            let linkTitle= linkRef.replace("heating-cooling-service-"+linkCityState,"Heating Cooling Service "+linkC+" "+linkS).replace("hvac-air-conditioning-repair-installation-services-"+linkCityState,"Hvac Air Conditioning Repair & Air Conditioning Installation Services "+linkC+" "+linkS).replace("hvac-furnace-repair-services-"+linkCityState,"Furnace Services "+linkC+" "+linkS);
            let linkText= linkRef.replace("heating-cooling-service-"+linkCityState,"Hvac Services "+linkC+" "+linkS).replace("hvac-air-conditioning-repair-installation-services-"+linkCityState,"A/C Services "+linkC+" "+linkS).replace("hvac-furnace-repair-services-"+linkCityState,"Furnace Services "+linkC+" "+linkS);
            linkArr = [...linkArr,{href:linkRef,title:linkTitle,text:linkText}]
        }
        return linkArr;
    };
    export let linkArr = landingLinksRand();
</script>
<style>
    footer {
        border-top: 8px solid #b0a990;
        background-color: #856e38;
        padding: 5em 2em;
        color: #fff;
        align-items:center;
        align-content:center;
        text-align:center;
        /* background: rgb(61, 84, 103);
        background: linear-gradient(161deg, rgba(61, 84, 103, 1) 0%, rgba(82, 108, 130, 1) 100%); */
    }
    .footer1{
        align-self:center;
    }
    .bottombar {
        background-color: #333333;
        padding: 1.25rem;
    }
    .footercontent {
        color: #fff;
    }
    .footernav-item {
        display: block;
        width: 100%;
        padding: .25rem 0rem;
        clear: both;
        font-weight: 400;
        color: #fff;
        font-weight: 300;
        font-family: 'Oswald', sans-serif;
    }
    .footercontent p {
        font-family: 'Oswald', sans-serif;
        font-weight: 300;
    }
    .footercontent a {
        color: #fff;
    }
    .footercontent a:hover {
        color: rgba(255, 255, 255, .75);
        text-decoration: none;
    }
    .bottombar .footercontent{
        align-items:center;
    }
</style>
<footer>
    <div class="container">
        <div class="row footercontent">
            <div class="col-sm footer1">
                <h3>Ultimate Plumbing</h3>
                <p>305 N Eric Dr # D<br>
                    Palatine, IL 60067</p>
                <h3><a href="tel:+1847-776-6001" title="Click Here To Call Now">(847) 776-6001</a></h3>
                <h3>Operating Hours</h3>
                Sunday: Closed <br>
                Monday: 6AM–5PM<br>
                Tuesday: 6AM–5PM<br>
                Wednesday: 6AM–5PM<br>
                Thursday: 6AM–5PM<br>
                Friday: 6AM–5PM<br>
                Saturday: 7AM–12PM
            </div>
            <div class="col-sm footer2">
                <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1513197.183287878!2d-89.96373091870048!3d42.20454280152865!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x880fa45f4e4e20c5%3A0xc983857383e256f4!2sUltimate%20Plumbing%20Supply!5e0!3m2!1sen!2sus!4v1570129603313!5m2!1sen!2sus" width="100%" height="450" frameborder="0" style="border:0;" allowfullscreen=""></iframe>
            </div>
<!--            <div class="col-sm footer3">-->
<!--                {#each linkArr as lk}-->
<!--                <a class="footernav-item" href='/{lk.href}' title="{lk.title}">{lk.text}</a>-->
<!--                {/each}-->
<!--            </div>-->
<!--            <div class="col-sm footer4">-->
<!--                <a class="footernav-item" href='reviews' title="Reviews">Reviews</a>-->
<!--                <a class="footernav-item" href='/special' title="Specials">Specials</a>-->
<!--                <a class="footernav-item" href='/maintenance' title="Maintenance">Maintenance</a>-->
<!--                <a class="footernav-item" href='/contact' title="Contact">Contact</a>-->
<!--            </div>-->
        </div>
    </div>
</footer>
<div class="bottombar">
    <div class="container">
        <div class="row footercontent">
            <div class="col-sm">
                &copy; 2019 All Rights Reserved
            </div>
            <div class="col-sm">
                <a href="https://insightweb.net" title="Site Designed By Insight Marketing Solutions">
                    <img src="/assets/images/designbyinsight.png" alt="Insight Marketing Solutions Inc Logo"/>
                </a>
            </div>
        </div>
    </div>
</div>
