<script>
    import Hero from '../../components/Hero.svelte';
    import SidebarSubnav from '../../components/SidebarSubnav.svelte';
    export let segment;
</script>
<style>
    .address{
        padding:2rem;
    }
</style>
<Hero
        heroImage="/assets/images/heros/homepage.jpg"
        heroTitle="Contact Ultimate Plumbing Supplies"
        heroBigText="Free Estimates"
        heroText=" Fill Out The Form Below Or Call To Contact Ultimate Plumbing Supplies">
    <p>Contact Ultimate Plumbing Supplies at <a href="tel:+1847-776-6001" title="click here to call now">1-847-776-6001</a>.</p>
    <a class="btn btn-light" href="/contact" title="Schedule Plumbing Repair Or Plumbing Installation Service">Order Now</a>
</Hero>
<div class="container">
    <div class="row">
        <section class="content col-xs-12 col-sm-8">
            <slot></slot>
        </section>
        <aside class="content col-xs-12 col-sm-4">
            <SidebarSubnav {segment}/>
        </aside>
    </div>
</div>