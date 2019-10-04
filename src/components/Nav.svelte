<script>
	export let segment;
</script>

<style>
	.bg-main-menu{
		background: linear-gradient(180deg, rgba(222,222,222,1) 0%, rgba(238,238,238,1) 49%, rgba(255,255,255,1) 100%);
	}
	.bg-image{
		width:300px;
		padding:2rem;
		align-self:center;
		display:flex;
		flex-direction:column;
		justify-content:center;
		background-color:grey;
		height:100%;
		color:#ffffff;
		text-align:center;
	}

	.bg-heatnav {
	background-size: cover;
	background-repeat: no-repeat;
	background-position: center;
	background-image: url("/assets/images/heatnav.jpg");
	}

	.bg-acnav {
	background-size: cover;
	background-repeat: no-repeat;
	background-position: center;
	background-image: url("/assets/images/acnav.jpg");
	}
	.dropdown-menu{
		min-width:600px;
		margin:0;
		padding:0;
	}
	.row{
		padding:0;
		margin:0;
	}
	.col-6{
		justify-content:center;
		display:flex;
		flex-direction:column;

	}
	.mega-content {
		padding:2em;
	}

	.nav{
		padding: 0;
	}
	.nav > li{
		min-height:50px;
		display:flex;
		flex-direction:column;
		font-family: 'Oswald', sans-serif;
		font-weight:700;


	}
	.nav > li > a{
		align-content:center;
		font-size:20px;
		text-transform:uppercase;
		color:#3d5467;
		font-weight:bold;
		border-right: 1px solid white;
		padding:1.25em 0 1.25em 0;
		border-radius:0;
		font-weight:700;
	}

	.nav > li > a:hover {
    background-color: #ffffff;
    text-decoration:none;
    }


	.nav > li:first-of-type > a{
		border-left: 1px solid white;
	}
	.nav > li > a:focus, .active{

		background-color:#7d0006 !important;
		color:white !important;
	}

	.dropdown-menu {
		border:none;
		border-radius:0 0 .25rem .25rem;
	}
	.dropdown-item.active:not(*:active) {
		color: var(--primary-color);
	}
	.dropdown-item:active:not(*:active) {
		color: var(--primary-color);
	}
</style>
<section class="bg-main-menu d-none d-md-block">
	<nav class="container">
		<ul class="nav navbar navbar-dark nav-fill nav-pills justify-content-between">
			<li class="nav-item dropdown">
			<a class="nav-link dropdown-toggle" href='#' role="button" aria-haspopup="true" aria-expanded="false" data-toggle="dropdown" title="Plumbing Parts Tools & Accessories">Plumbing</a>
				<div class="dropdown-menu">
					<div class="row">
							<div class="col-6 mega-content">
								<h3>Plumbing</h3>
								<a rel=prefetch class='dropdown-item {segment === "backflow-prevention" ? "active" : ""}' href='backflow-prevention' title="Backflow Prevention Systems">Backflow Prevention</a>
								<a rel=prefetch class='dropdown-item {segment === "backup-systems" ? "active" : ""}' href='backup-systems' title="Backup Plumbing Systems">Backup Systems</a>
								<a rel=prefetch class='dropdown-item {segment === "pipes-accessories" ? "active" : ""}' href='pipes-accessories' title="Plumbing Pipes & Accessories">Pipes &amp; Accessories</a>
								<a rel=prefetch class='dropdown-item {segment === "plumbing-fittings" ? "active" : ""}' href='plumbing-fittings' title="Plumbing Fittings">Fittings</a>
								<a rel=prefetch class='dropdown-item {segment === "plumbing-fixtures" ? "active" : ""}' href='plumbing-fixtures' title="Plumbing Fixtures">Fixtures</a>
								<a rel=prefetch class='dropdown-item {segment === "plumbing-tools" ? "active" : ""}' href='plumbing-tools' title="Plumbing Tools">Tools</a>
							</div>
							<div class="col-6">
								<div class="bg-image bg-heatnav">

								</div>
							</div>
						</div>
				</div>
			</li>
			<li class="nav-item"><a rel=prefetch href='commercial-restaurant-plumbing-equipment' title="Cooling">Restaurant Equipment</a></li>
			<li class="nav-item"><a rel=prefetch class='{segment === "plumbing-pumps" ? "active" : ""}' href='plumbing-pumps' title="Sump Pumps, Ejector Pumps, Grinder Pumps, Booster Pumps">Pumps</a></li>
			<li class="nav-item"><a rel=prefetch class='{segment === "water-heaters" ? "active" : ""}' href='water-heaters' title="Water Heaters">Water Heaters</a></li>
			<li class="nav-item"><a rel=prefetch class='{segment === "about-us" ? "active" : ""}' href='about-us' title="About Ultimate Plumbing">About Us</a></li>
			<li class="nav-item"><a rel=prefetch class='{segment === "contact" ? "active" : ""}' href='contact' title="Contact Us">Contact</a></li>
		</ul>
	</nav>
</section>

