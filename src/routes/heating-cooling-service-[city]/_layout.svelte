<script context="module">
    export async function preload({params, query}){
        // return this.fetch(`/nn-filler.html/`)
        // 		.then((r) => {
        // 			r.text().then((nnText) =>{
        // 				return content = nnText;
        // 			});
        // 		})
        let cs = await params.city.split("-");
        let state = await cs[cs.length - 1].toUpperCase();
        let city = await params.city.replace("-"+state.toLowerCase(),'').replace('-',' ').replace(params.city.substr(0,1),params.city.substr(0,1).toUpperCase());
        return {nnCity:city,nnState:state};
    }
</script>
<script>
    import Hero from '../../components/Hero.svelte';
    import CouponSidebar from '../../components/CouponSidebar.svelte';
    import SidebarSubnav from '../../components/SidebarSubnav.svelte';
    let locations;
    export let nnCity;
    let nnState="IL";
</script>
<style>

</style>
<Hero heroImage="/assets/images/heros/achero1.jpg" heroTitle="Aries Mechanical" heroBigText="Heating and Cooling Service near {nnCity}, {nnState}" heroText=" Your {nnCity}, {nnState} Furnace & Air Conditioner Repair Company">
    <p>Aries Mechanical is a licensed, insured, and bonded hvac, heating, and cooling company that services the {nnCity}, {nnState} area.</p>
    <a class="btn btn-light" href="/contact" title="Schedule Hvac Repair Or Hvac Installation Service">Order Now</a>
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
