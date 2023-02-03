<script>
    import Hero from '../../components/Hero.svelte';
    import SidebarSubnav from '../../components/SidebarSubnav.svelte';
</script>
<style>

</style>
<Hero
        heroImage="/assets/images/heros/waterheaters.jpg"
        heroTitle="Water Heaters"
        heroBigText="Affordable & Quality Water Heaters"
        heroText=" Your Plumbing Equipment &amp; Supplies Company">
    <a class="btn btn-light" href="/contact" title="Order Your Water Heater Now">Order Your New Water Heater Now</a>
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
