<script>
    import Hero from '../../components/Hero.svelte';
    import SidebarSubnav from '../../components/SidebarSubnav.svelte';
</script>
<style>

</style>
<Hero
        heroImage="/assets/images/heros/fittings.jpg"
        heroTitle="Programmable Thermostats"
        heroBigText="Affordable & High Quality Plumbing Supplies"
        heroText="Premier Plumbing Supplier">
    <p>Same Day Delivery Now Available!</p>
    <a class="btn btn-light" href="/contact" title="Get Your Plumbing Fittings With Same Day Delivery Now">Order Now</a>
</Hero>
<div class="container">
    <div class="row">
        <section class="content col-xs-12 col-sm-8">
            <slot></slot>
        </section>
        <aside class="content col-xs-12 col-sm-4">
            <SidebarSubnav />
        </aside>
    </div>
</div>
