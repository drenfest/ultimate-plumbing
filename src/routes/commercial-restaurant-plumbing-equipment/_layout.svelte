<script>
         import Hero from '../../components/Hero.svelte';
      import ProductGuide from '../../components/ProductGuide.svelte';
     import SidebarSubnav from '../../components/SidebarSubnav.svelte';
</script>
<style>

</style>
<Hero
        heroImage="/assets/images/heros/achero1.jpg"
        heroTitle="Ultimate Plumbing"
        heroBigText="Commercial Restaurant Plumbing Equipment"
        heroText="For All Your Plumbing Needs">
    <a class="btn btn-light" href="/contact" title="Schedule Hvac Repair Or Hvac Installation Service">Order Equipment Now</a>
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
