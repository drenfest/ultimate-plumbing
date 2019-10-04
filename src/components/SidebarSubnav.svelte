<script>
export let segment ="";
</script>
<style>
    .sidebar-subnav {
        padding: 2rem 1rem;
    }

    .sidebar-subnav ul {
       margin: 0;
    padding: 0;
    list-style-type: none;
    font-family: 'Oswald', sans-serif;
    font-size: 14px;
    /* border: 2px solid var(--success); */
    background-color: #efefef;
    padding: 15px 0px;
    background-image:url("/assets/images/subnavbk.png");
    background-position:bottom right;
   background-repeat: no-repeat;


    }

    .sidebar-subnavli {
        margin: 0 0 3px 0;
    }

    .sidebar-subnav a {
    display: block;
    padding: .25rem 0rem;
    font-weight: 400;
    color: var(--success);
    font-size: 22px;
    font-family: 'Oswald', sans-serif;
    text-transform: uppercase;
    padding: .5rem 2rem;
    }

    .sidebar-subnav a:hover {
        background-color:transparent;
        color: var(--primary-color);
        text-decoration: none;
    }

</style>
<section class="sidebar-subnav">
    <ul>
        <li><a rel=prefetch class='dropdown-item {segment === "backflow-prevention" ? "active" : ""}' href='backflow-prevention' title="Backflow Prevention Systems">Backflow Prevention</a></li>
        <li><a rel=prefetch class='dropdown-item {segment === "backup-systems" ? "active" : ""}' href='backup-systems' title="Backup Plumbing Systems">Backup Systems</a></li>
        <li><a rel=prefetch class='dropdown-item {segment === "pipes-accessories" ? "active" : ""}' href='pipes-accessories' title="Plumbing Pipes & Accessories">Pipes &amp; Accessories</a></li>
        <li><a rel=prefetch class='dropdown-item {segment === "plumbing-fittings" ? "active" : ""}' href='plumbing-fittings' title="Plumbing Fittings">Fittings</a></li>
        <li><a rel=prefetch class='dropdown-item {segment === "plumbing-fixtures" ? "active" : ""}' href='plumbing-fixtures' title="Plumbing Fixtures">Fixtures</a></li>
        <li><a rel=prefetch class='dropdown-item {segment === "plumbing-tools" ? "active" : ""}' href='plumbing-tools' title="Plumbing Tools">Tools</a></li>
        <li><a rel=prefetch href='commercial-restaurant-plumbing-equipment' title="Restaurant Equipment">Restaurant Equipment</a></li>
        <li><a rel=prefetch class='{segment === "plumbing-pumps" ? "active" : ""}' href='plumbing-pumps' title="Sump Pumps, Ejector Pumps, Grinder Pumps, Booster Pumps">Pumps</a></li>
        <li><a rel=prefetch class='{segment === "water-heaters" ? "active" : ""}' href='water-heaters' title="Water Heaters">Water Heaters</a></li>
        <li><a rel=prefetch class='{segment === "about-us" ? "active" : ""}' href='about-us' title="About Ultimate Plumbing">About Us</a></li>
        <li><a rel=prefetch class='{segment === "contact" ? "active" : ""}' href='contact' title="Contact Us">Contact</a></li>
    </ul>
</section>
