<script>
    import Hero from '../../components/Hero.svelte';
    import ProductGuide from '../../components/ProductGuide.svelte';
    import SidebarSubnav from '../../components/SidebarSubnav.svelte';
    export let segment;
</script>
<style>
    .address{
        padding:2rem;
    }
</style>
<Hero
        heroImage="/assets/images/heros/hmhero1.jpg"
        heroTitle="Affordable & High Quality Plumbing Supplies"
        heroBigText="Contact Ultimate Plumbing"
        heroText=" Fill Out The Form Below Or Call To Contact Ultimate Plumbing">
    <p>Contact Ultimate Plumbing at (847) 776-6001. We are located at 305 N Eric Dr # D, Palatine, IL 60067</p>
    <a class="btn btn-light" href="/contact" title="Schedule Hvac Repair Or Hvac Installation Service">Order Now</a>
</Hero>
<div class="container">
    <div class="row">
        <section class="content col-xs-12 col-sm-8">
            <slot></slot>
        </section>
        <aside class="content col-xs-12 col-sm-4">
            <div class="address">
                <h2>Contact Info</h2>
                <strong>Address: </strong>
                <address>
                    305 N Eric Dr # D, Palatine, IL 60067
                </address>
                <strong>Phone: </strong><a href="tel:+1847-776-6001">(847) 776-6001</a>
            </div>
            <SidebarSubnav {segment}/>
        </aside>
    </div>
</div>
