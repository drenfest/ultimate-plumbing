<script>
	import Hero from '../components/Hero.svelte';
	import Divider from '../components/Divider.svelte';
	import Coupon from '../components/Coupon.svelte';
	import TraneBanner from '../components/TraneBanner.svelte';
	import ServicesGrid from '../components/ServicesGrid.svelte';

</script>
<style>
	.about-section{
		padding:4rem 2rem;
		background-image: url(/assets/images/homeaboutbk-m.jpg);
		background-size: cover;
		background-position: bottom center;
	}
	.about-section > .container > h2{
		margin-bottom:1.75rem;
		font-weight:700;
		font-size:2.5rem;
	}
	.aboutsub {
	font-size:60%;
	font-weight:300;
	display:block;
	text-transform:uppercase;
	}

	.about-support {
	font-family: 'Oswald', sans-serif;
	text-transform:uppercase;
	font-size:18px;
	font-weight:400;
	line-height:1.4em;
	display:block;
	margin-bottom:.15rem;
	}
	.abouthmtx {
	padding:0px ;
	}

	.service-btns-bg{
	background: rgb(61,84,103);
background: linear-gradient(90deg, rgba(61,84,103,1) 9%, rgba(96,115,130,1) 90%);
	}
	.service-buttons{
		display:grid;
		grid-template-rows:1fr 1fr 1fr;
	}
	.coupon-section{
		background: #e6e6e6;
		padding:3rem 0;
	}
	.specials-button{
		margin-top:2rem;
	}
	.specials-button>a{
		background-color:var(--primary-color);
		border:none;
		border-radius:0;
	}
	.specials-button>a:hover{
		background-color:#711D1D;
	}
	@media screen and (min-width:768px){

	.about-section{
		padding:6rem 2rem;
		background-image: url(/assets/images/homeaboutbk.jpg);
		background-size: cover;
		background-position: bottom center;
	}
	.abouthmtx {
	padding:0px 75px;
	}


		.service-btns-bg{
			background: rgb(61,84,103);
background: linear-gradient(90deg, rgba(61,84,103,1) 9%, rgba(96,115,130,1) 90%);
		}
		.service-buttons{
			grid-template-rows:1fr;
			grid-template-columns: 1fr 1fr 1fr;
			max-width: 1140px;
			margin:auto;
		}
	}
</style>
<svelte:head>
	<title>Ultimate Plumbing | Premier Plumbing Parts, Tools, & Accessories Provider</title>
	<meta name="description" content="Top Rated Plumbing Supply Company">
</svelte:head>
<Hero
		heroImage="/assets/images/heros/homepagepic.jpg"
		heroTitle="Ultimate Plumbing Supply"
		heroBigText="Affordable & High Quality Plumbing Parts & Tools"
		heroText="Same Day Delivery Available!">
	<p>If we don’t have the part you are looking for… It probably hasn’t been invented yet.</p>
	<a class="btn btn-light" href="/contact" title="Order Your Plumbing Tool Or Part">Order Your Part/Tool Now</a>
</Hero>
<!--Service Buttons Are In Hero Component-->
<section class="about-section">
	<div class="container"><h2 class="text-center">Ultimate Plumbing<span class="aboutsub">Preferred Plumbing Parts &amp; Tools Supplier</span>
	</h2>
		<div class="row">
			<div class="col-xs-12"><p>Ultimate Plumbing Supply has been serving the Palatine &amp; Arlington Heights IL
				area for over 25 years. We are a full service plumbing supplier serving Lake, Cook, McHenry, Kane and
				Dupage counties. We take pride in working with customers on any project from the smallest do it yourself
				to complete remodels. We can assist with home and commercial construction projects. We offer high
				quality plumbing supplies &amp; parts for homeowners, contractors and plumbers. No matter what the job,
				homeowner, apartment building, restaurant, large retail business or any other facility with multiple
				bathrooms or kitchens, give Ultimate Plumbing Supply a call today.</p></div>
		</div>
		<iframe allowfullscreen="" frameborder="0" height="450"
				src="https://www.youtube.com/embed/NTESMdKjnhk"
				width="100%" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"></iframe>
		<div class="row justify-content-center"><p class="svelte-nw229z about-support">Free
			Estimates | 24/7 Support </p></div>
		<div class="row justify-content-center"><a
				href="tel:+1847-776-6001" title="Click Here To Call Now "
				class="btn btn-primary text-center">Call Now! (847)776-6001</a></div>
	</div>
</section>
<Divider>
	<h2>Plumbing Parts Tools &amp; Accessories </h2>
</Divider>
<ServicesGrid/>
