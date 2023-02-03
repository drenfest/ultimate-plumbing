<script>
         import Hero from '../../components/Hero.svelte';
      import ProductGuide from '../../components/ProductGuide.svelte';
     import SidebarSubnav from '../../components/SidebarSubnav.svelte';
</script>
<style>

</style>
<Hero
        heroImage="/assets/images/heros/backflow-prevention.jpg"
        heroTitle="Ultimate Plumbing"
        heroBigText="Backflow Prevention Systems"
        heroText="Get Control Of Your Plumbing Backflow">
    <p>Same Day Delivery Available!</p>
    <a class="btn btn-light" href="/contact" title="Order Your Backflow Prevention System Now">Order Your Backflow Prevention System Now</a>
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
