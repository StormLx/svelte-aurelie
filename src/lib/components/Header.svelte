<script lang="ts">
    import logo from '$lib/assets/logo.svg';
</script>

<header id="header" class="d-flex align-items-center" data-aos="fade-down" data-aos-duration="300ms">
    <div class="container-fluid container-xl d-flex align-items-center justify-content-lg-between">

        <h1 class="logo me-auto me-lg-0">
            <a href="/" class="d-flex align-items-center justify-content-center">
                <span>Aurélie Millet</span>
                <img src="{logo}" alt="logo" height="50px" class="small-white-logo"></a>
        </h1>

        <nav id="navbar" class="navbar order-last order-lg-0">
            <ul>
                <li><a class="nav-link scrollto active" href="/">Accueil</a></li>
                <li><a class="nav-link scrollto" href="/presentation">Présentation</a></li>
                <li><a class="nav-link scrollto" href="/accompagnements">Mes accompagnements</a></li>
                <li><a class="nav-link scrollto" href="/pourquoi">Pour quoi, pour qui</a></li>
                <li><a class="nav-link scrollto" href="/seances">Les séances</a></li>
            </ul>
            <i class="bi bi-list mobile-nav-toggle"></i>
        </nav>
        <a href="/contact" class="book-a-table-btn scrollto d-none d-lg-flex">Contact</a>
    </div>
</header>

<style>
    #header {
        background: rgba(12, 11, 9, 0.6);
        border-bottom: 1px solid rgba(12, 11, 9, 0.6);
        transition: all 0.5s;
        z-index: 997;
        padding: 15px 0;
        animation: 1s ease-out forwards slideMenuDown;
    }

    #header .logo {
        color: var(--white-color);
        font-size: 20px;
        margin: 0;
        padding: 0;
        line-height: 1;
        font-weight: 400;
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


    /*--------------------------------------------------------------
    # Navigation Menu
    --------------------------------------------------------------*/
    /**
    * Desktop Navigation
    */
    .navbar {
        padding: 0;
    }

    .navbar ul {
        margin: 0;
        padding: 0;
        display: flex;
        list-style: none;
        align-items: center;
    }

    .navbar li {
        position: relative;
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

    .navbar a i {
        font-size: 12px;
        line-height: 0;
        margin-left: 5px;
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

    .navbar .dropdown ul a i {
        font-size: 12px;
    }

    .navbar .dropdown ul a:hover, .navbar .dropdown ul .active:hover, .navbar .dropdown ul li:hover > a {
        color: var(--secondary-color-lighter);
    }


    .navbar .dropdown .dropdown ul {
        top: 0;
        left: calc(100% - 30px);
        visibility: hidden;
    }


    @media (max-width: 1366px) {
        .navbar .dropdown .dropdown ul {
            left: -90%;
        }
    }

    /**
    * Mobile Navigation
    */
    .mobile-nav-toggle {
        color: var(--white-color);
        font-size: 28px;
        cursor: pointer;
        display: none;
        line-height: 0;
        transition: 0.5s;
    }

    @media (max-width: 991px) {
        .mobile-nav-toggle {
            display: block;
        }

        .navbar ul {
            display: none;
        }
    }


    .navbar-mobile .dropdown ul li {
        min-width: 200px;
    }

    .navbar-mobile .dropdown ul a {
        padding: 10px 20px;
    }

    .navbar-mobile .dropdown ul a:hover, .navbar-mobile .dropdown ul .active:hover, .navbar-mobile .dropdown ul li:hover > a {
        color: var(--secondary-color-lighter);
    }


    @-webkit-keyframes animate-loading {
        0% {
            transform: rotate(0deg);
        }
        100% {
            transform: rotate(360deg);
        }
    }

    @keyframes animate-loading {
        0% {
            transform: rotate(0deg);
        }
        100% {
            transform: rotate(360deg);
        }
    }
</style>
