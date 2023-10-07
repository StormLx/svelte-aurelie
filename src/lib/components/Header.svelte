<script lang="ts">
    import logo from '$lib/assets/logo.svg';
    import { page } from '$app/stores';

    $: path = $page.route.id;
</script>

<header id="header">
    <nav class="navbar navbar-expand-lg">
        <h1 class="logo me-auto me-lg-0">
            <a href="/" class="d-flex align-items-center justify-content-center">
                <h4 class="m-0">Aurélie Millet</h4>
                <img src="{logo}" alt="logo" height="50px" class="small-white-logo"></a>
        </h1>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavDropdown"
                aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNavDropdown">
            <ul class="navbar-nav">
                <li class="nav-item" class:active={path === '/'}><a class="nav-link" href="/">Accueil</a></li>
                <li class="nav-item" class:active={path === '/presentation'}><a class="nav-link" href="/presentation">Présentation</a></li>
                <li class="nav-item" class:active={path === '/accompagnements'}><a class="nav-link" href="/accompagnements">Mes accompagnements</a></li>
                <li class="nav-item" class:active={path === '/pourquoi'}><a class="nav-link" href="/pourquoi">Pour quoi, pour qui</a></li>
                <li class="nav-item" class:active={path === '/contact'}><a class="nav-link" href="/contact">Tarif & Contact</a></li>
            </ul>
        </div>
    </nav>
</header>


<style>
    .navbar-toggler {
        background-color: var(--white-color);
        margin-right: 10px;

        &:active {
            transform: scale(0.95);
        }
    }

    #header {
        background: rgba(12, 11, 9, 0.6);
        border-bottom: 1px solid rgba(12, 11, 9, 0.6);
        transition: all 0.5s;
    }

    #header .logo {
        margin: 0;
        padding: 0;
        letter-spacing: 1px;
        text-transform: uppercase;
    }

    .small-white-logo {
        color: white;
        width: 50px;
        display: block;
    }

    #header .logo a {
        color: var(--white-color);
    }

    #header .logo img {
        max-height: 40px;
    }


    .navbar a {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 10px 0 10px 30px;
        color: var(--white-color);
        white-space: nowrap;
        transition: 0.3s;
        font-size: 14px;
    }


    .navbar a:hover, .navbar .active, .navbar li:hover > a {
        color: var(--secondary-color-lighter);
    }

    .navbar .dropdown ul {
        display: block;
        position: absolute;
        left: 14px;
        top: calc(100% + 30px);
        margin: 0;
        padding: 10px 0;
        z-index: 99;
        opacity: 0;
        visibility: hidden;
        color: var(--white-color);
        box-shadow: 0px 0px 30px rgba(127, 137, 161, 0.25);
        transition: 0.3s;
        border-radius: 4px;
    }

    .navbar .dropdown ul li {
        min-width: 200px;
    }

    .navbar .dropdown ul a {
        padding: 10px 20px;
        color: #444444;
    }

    .navbar .dropdown ul a:hover, .navbar .dropdown ul .active:hover, .navbar .dropdown ul li:hover > a {
        color: var(--secondary-color-lighter);
    }


    .navbar .dropdown .dropdown ul {
        top: 0;
        left: calc(100% - 30px);
        visibility: hidden;
    }

</style>
