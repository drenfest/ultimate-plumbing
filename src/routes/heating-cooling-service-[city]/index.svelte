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
	export let nnCity;
	export let nnState;
	export let locations = [
		{city:"Bristol", state:"IL"},
		{city:"Lisbon", state:"IL"},
		{city:"Millbrook", state:"IL"},
		{city:"Newark", state:"IL"},
		{city:"Norway", state:"IL"},
		{city:"Oswego", state:"IL"},
		{city:"Ottawa", state:"IL"},
		{city:"Plano", state:"IL"},
		{city:"Sandwich", state:"IL"},
		{city:"Sheridan", state:"IL"},
		{city:"Somonauk", state:"IL"},
		{city:"Sugar grove", state:"IL"},
		{city:"Yorkville", state:"IL"},
	];
</script>
<style>
</style>
<svelte:head>
	<title> Heating and Cooling Service near {nnCity}, {nnState}</title>
	<meta name="description" content="Aries Mechanical is a licensed, insured, and bonded hvac, heating, and cooling company that services the {nnCity}, {nnState} area.">
</svelte:head>
<h2>Heating and Cooling Service</h2>
<p>Aries Mechanical is a licensed, insured, and bonded HVAC company that services the {nnCity}, {nnState} area. We have been installing, repairing and maintaining air conditioning units, heating units, and furnaces in {nnCity}, {nnState} for many years.</p>
<p>We have worked hard to provide our customers with the best possible air conditioning service at the most reasonable prices. Emergency Air Conditioning Repair Services are available 24 hours a day, 7 days a week for any HVAC emergency.</p>
<h3>Furnace Repair &amp; Installation in {nnCity}, {nnState}</h3>
<p>Whether you are looking for gas furnace service or repair, quality installation of a furnace, heat pump or air conditioner, endless hot water from tankless water heaters, better air quality in your home or just a filter change or duct cleaning, Aries Mechanical is your best choice of {nnCity}, {nnState} heating contractors and cooling specialists.</p>
<p>Aries Mechanical offers service throughout the {nnCity}, {nnState} area. If you are not currently receiving regular maintenance on your heating system, what are you waiting for? Give us a call at Aries Mechanical today. If you want your heating system to continue working through the colder months, it is important that you receive routine maintenance. This also prevents more expensive repairs in the future. Routinely performed maintenance will help to keep your heating unit functioning effectively and efficiently.</p>
<p>To find out more about our services, we have associates who will be able to offer you information about our processes for helping to keep your heating unit in tip top condition. They will explain the many benefits of having your system routinely serviced. {nnCity}, {nnState} has many heating and cooling providers, but why not turn to the service that is preferred, Aries Mechanical.</p>
<h3>Air Conditioning Repair &amp; Maintenance</h3>
<p>The most trusted {nnCity}, {nnState} area HVAC service is Aries Mechanical. Making sure that your air conditioning is always working properly will require routine maintenance. Make sure you only call on the services of a trained and qualified professional to handle the job of offering you the maintenance that you need in order for your air conditioner to continue working the way that it should. It is not uncommon for your air conditioner to begin giving you problems during warmer months. Although an extremely frustrated occurrence, there is no need to panic. Simply call on the expert services of Aries Mechanical.</p>
<p>Costly air conditioner repair can be avoided by replacing your air filter every 60 days. As every AC Repair issue is unique, we always come to your home to assess the problem and give you a detailed estimate rather than trying to diagnose the problem over the phone. We present both repair and replacement options fairly, keeping the customer&rsquo;s interests in mind, and always wait for the homeowner&rsquo;s OK before proceeding with the AC repair. If any issues come up during the repair visit, we communicate clearly with the homeowner right away. For any and all of your air conditioner repair in {nnCity}, {nnState} contact us. We provide same day air conditioner repair and 24 hours emergency air conditioning repair service.</p>
<p>We install a variety of home comfort systems, and we provide <strong>24/7 emergency repairs</strong>.</p>
<strong>Call the heating and air conditioning experts at Aries Mechanical to learn more about our residential and commercial HVAC services in the {nnCity}, {nnState} area. We are here to serve you in any way we can, so call today!</strong>
