<script>
    import Hero from '../../components/Hero.svelte';
    import ProductGuide from '../../components/ProductGuide.svelte';
    import SidebarSubnav from '../../components/SidebarSubnav.svelte';
</script>
<style>
</style>
<Hero
        heroImage="/assets/images/heros/plumbing-supplies.jpg"
        heroTitle="Affordable & High Quality Plumbing Supplies"
        heroBigText="Plumbing Fixtures"
        heroText="Premier Plumbing Supplier">
    <p>Same Day Delivery Now Available!</p>
    <a class="btn btn-light" href="/contact" title="Call Us Now To Get Started">Call Us Now To Get Started</a>
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
