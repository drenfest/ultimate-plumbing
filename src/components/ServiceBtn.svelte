<script>
    export let serviceBtnBg = "#ec3237";
    export let serviceLink, serviceTitle, serviceIcon, serviceIconAlt;
</script>
<style>
    .service-btn > a{
        text-decoration:none;
        display:grid;
        grid-template-columns: 30% 60% 10%;
        color:white;
        padding:1rem;
        align-items:center;
        font-size:30px;
        font-family: 'Oswald', sans-serif;
        text-align:center;

    }
    .service-btn > a:hover{
        text-decoration:none;

    }
    .service-btn > a > img{
        border-right:1px solid white;
        padding-right:2rem;
    }
    .greater-than{
        font-weight:bold;
    }
</style>
<div class="service-btn" style="background-color:{serviceBtnBg};">
    <a href="{serviceLink}" title="{serviceTitle}">
        <img src="{serviceIcon}" alt="{serviceIconAlt}"/>
        <slot></slot>
        <div class="greater-than">&gt;</div>
    </a>
</div>
