<script>

</script>
<style>
    .grid{
        display:grid;
        grid-template-columns: 1fr;
        grid-gap:1rem;
        text-align:center;
        padding:3rem 1rem;
    }
    .service{
        display:flex;
        flex-direction:column;
        justify-content:center;
        min-height:300px;
        max-height:300px;
        font-size:2rem;
        color:white;
        font-weight:bold;
        background-color:rgba(0,0,0,.4);
        background-blend-mode:overlay;
        font-family: 'Oswald', sans-serif;
        background-size: cover;
        background-position: center center;

    }
    .service-heating{
        background-image:url("/assets/images/services/service1.jpg");
    }
    .service-ac{
        background-image:url("/assets/images/services/service2.jpg");
    }
    .service-air-cleaning{
        background-image:url("/assets/images/services/service3.jpg");
    }
    .service-res-hvac{
        background-image:url("/assets/images/services/service4.jpg");
    }
    .service-humidify{
        background-image:url("/assets/images/services/service-humidification.jpg");
    }
    .service-thermostats{
        background-image:url("/assets/images/services/service5.jpg");
    }
    @media screen and (min-width:768px){
        .grid{
            grid-template-columns: 1fr 1fr;
        }
    }
    @media screen and (min-width:992px){
        .grid{
            grid-template-columns: 1fr 1fr 1fr;
        }
    }
</style>
<section class="services-grid">
    <div class="container">
        <div class="grid">
            <a class="service service-heating" title="Backflow Prevention" href="/backflow-prevention">Backflow Prevention</a>
            <a class="service service-ac" title="Plumbing Backup Systems" href="/backup-systems">Backup Systems</a>
            <a class="service service-air-cleaning" title="Plumbing Pipes & Accessories" href="/pipes-accessories">Pipes &amp; Accessories</a>
            <a class="service service-res-hvac" title="Plumbing Fittings" href="/plumbing-fittings">Fittings</a>
            <a class="service service-thermostats" title="Plumbing Fixtures" href="/plumbing-fixtures">Fixtures</a>
            <a class="service service-humidify" title="Sump Pumps, Ejector Pumps, Grinder Pumps, Booster Pumps" href="/plumbing-pumps">Pumps</a>
            <a class="service service-res-hvac" title="Plumbing Tools" href="/plumbing-tools">Tools</a>
            <a class="service service-thermostats" title="Water Heaters" href="/water-heaters">Water Heaters</a>
            <a class="service service-humidify" title="Commercial Restaurant Plumbing Equipment" href="/commercial-restaurant-plumbing-equipment">Restaurant Equipment</a>
        </div>
    </div>
</section>
