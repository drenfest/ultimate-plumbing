<script>
    import Hero from '../../components/Hero.svelte';
    import ProductGuide from '../../components/ProductGuide.svelte';
     import SidebarSubnav from '../../components/SidebarSubnav.svelte';
</script>
<style>

</style>
<Hero heroImage="/assets/images/heros/homepage.jpg"
      heroTitle="High Quality & Affordable"
      heroBigText="Plumbing Pumps"
      heroText="We are here to answer any questions you may have.">
    <a class="btn btn-light" href="/contact" title="Get Same Day Delivery By Ordering Your Plumbing Pump Now">Order Your Plumbing Pump Now</a>
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
