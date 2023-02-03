<script>

</script>
<style>
    .trane-banner a {
        color: white
    }

    .trane-banner a:hover {
        color: black
    }

    .grid {
        display: grid;
        grid-template-columns: 1fr;
        grid-gap: 1rem;
        text-align: center;
        padding: 3rem 1rem
    }

    .service {
        display: flex;
        flex-direction: column;
        justify-content: center;
        min-height: 300px;
        max-height: 300px;
        font-size: 2rem;
        color: white;
        font-weight: bold;
        background-color: rgba(0,0,0,.4);
        background-blend-mode: overlay;
        font-family: 'Oswald', sans-serif;
        background-size: cover;
        background-position: center center
    }

    .service-backflow-prevention {
        background-image: url("/assets/images/services/backflow-prevention-square.jpg")
    }

    .service-backup-systems {
        background-image: url("/assets/images/services/backup-systems-square.png")
    }

    .service-plumbing-accessories {
        background-image: url("/assets/images/services/pipes-square.jpg")
    }

    .service-plumbing-fittings {
        background-image: url("/assets/images/services/fittings-square.jpg")
    }

    .service-plumbing-fixtures {
        background-image: url("/assets/images/services/fixtures-square.jpg")
    }

    .service-pumps {
        background-image: url("/assets/images/services/sump-pumps-square.jpg")
    }

    .service-plumbing-tools {
        background-image: url("/assets/images/services/tools-square.jpg")
    }

    .service-water-heaters {
        background-image: url("/assets/images/services/waterheaters-square.jpg")
    }

    .service-restaurant-equipment {
        background-image: url("/assets/images/services/restaurant-equipment-square.jpg")
    }

    @media screen and (min-width: 768px) {
        .grid {
            grid-template-columns:1fr 1fr
        }
    }

    @media screen and (min-width: 992px) {
        .grid {
            grid-template-columns:1fr 1fr 1fr
        }
    }


    .about-section>.container>h2 {
        margin-bottom: 1.75rem;
        font-weight: 700;
        font-size: 2.5rem
    }

    .specials-button>a {
        background-color: var(--primary-color);
        border: none;
        border-radius: 0
    }

    .specials-button>a:hover {
        background-color: #711D1D
    }

    @media screen and (min-width: 768px) {

    }

</style>
<section class="services-grid">
    <div class="container">
        <div class="grid"><a href="/backflow-prevention" title="Backflow Prevention"
                                            class="service service-backflow-prevention">Backflow
            Prevention</a> <a href="/backup-systems" title="Plumbing Backup Systems"
                              class="service service-backup-systems">Backup Systems</a> <a
                href="/pipes-accessories" title="Plumbing Pipes &amp; Accessories"
                class="service service-plumbing-accessories">Pipes &amp; Accessories</a> <a
                href="/plumbing-fittings" title="Plumbing Fittings"
                class="service service-plumbing-fittings">Fittings</a> <a href="/plumbing-fixtures"
                                                                                         title="Plumbing Fixtures"
                                                                                         class="service service-plumbing-fixtures">Fixtures</a>
            <a href="/plumbing-pumps" title="Sump Pumps, Ejector Pumps, Grinder Pumps, Booster Pumps"
               class="service service-pumps">Pumps</a> <a href="/plumbing-tools" title="Plumbing Tools"
                                                                         class="service service-plumbing-tools">Tools</a>
            <a href="/water-heaters" title="Water Heaters" class="service service-water-heaters">Water
                Heaters</a> <a href="/commercial-restaurant-plumbing-equipment"
                               title="Commercial Restaurant Plumbing Equipment"
                               class="service service-restaurant-equipment">Restaurant Equipment</a>
        </div>
    </div>
</section>
