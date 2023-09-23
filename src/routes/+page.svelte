

<section id="hero" class="d-flex align-items-center">
    <div class="container text-center text-lg-start">
        <div class="row">
            <div class="col-lg-7 hero-title">
                <h1>Aurélie <span>Millet</span></h1>
                <div class="btns">
                    <a href="#presentation" class="btn-menu">Présentation</a>
                    <a href="#contact" class="btn-book">Contact</a>
                </div>
            </div>

            <div class="round-img">
            </div>
        </div>
    </div>
</section>

<style>
    #hero {
        width: 100%;
        height: calc(100vh - 72px);
        position: relative;
        padding: 0;
        overflow: hidden;
    }

    /* Background Image with Overlay */
    #hero::before {
        content: '';
        position: absolute;
        top: 0;
        right: 0;
        bottom: 0;
        left: 0;
        background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), url('$lib/assets/hero.jpg');
        background-size: cover;
        z-index: -1;
    }


    #hero .container {
        padding-top: 110px;
    }

    @media (max-width: 992px) {
        #hero .container {
            padding-top: 98px;
        }
    }

    #hero h1 {
        margin: 0;
        font-size: 64px;
        font-weight: 700;
        line-height: 56px;
        color: #fff;
    }

    #hero h1 span {
        color: var(--secondary-color);
    }

    #hero .btns {
        margin-top: 30px;
    }

    #hero .btn-menu, #hero .btn-book {
        font-weight: 600;
        font-size: 13px;
        letter-spacing: 0.5px;
        text-transform: uppercase;
        display: inline-block;
        padding: 12px 30px;
        border-radius: 50px;
        transition: 0.3s;
        line-height: 1;
        color: white;
        border: 2px solid var(--secondary-color);
    }

    #hero .btn-menu:hover, #hero .btn-book:hover {
        background: var(--secondary-color);
        color: #fff;
    }

    #hero .hero-title {
        display: flex;
        flex-direction: column;
        justify-content: center;
    }

    #hero .round-img {
        height: 400px;
        width: 400px;
        border-radius: 50%;
        position: relative;
    }

    #hero .round-img::before {
        content: '';
        position: absolute;
        border-radius: 50%;
        top: 0;
        right: 0;
        bottom: 0;
        left: 0;
        background-image: url('$lib/assets/profil.jpg');
        background-position: center;
        background-size: cover;
        z-index: 2;
    }

    #hero .round-img::after {
        content: '';
        position: absolute;
        border-radius: 50%;
        top: -90px;
        right: 0;
        bottom: 90px;
        left: 0;
        background: var(--secondary-color);
        opacity: 0.8;
        z-index: 1;
    }


    @media (min-width: 1024px) {
        #hero {
            background-attachment: fixed;
        }
    }

    @media (max-width: 992px) {
        #hero {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }

        #hero .row {
            flex-direction: column;
            align-items: center;
            justify-content: center;
            gap: 30px;
        }

        #hero .round-img {
            margin-top: 100px;
            height: 300px;
            width: 300px;
        }
    }

    @media (max-height: 500px) {
        #hero {
            height: auto;
        }
        #hero .container {
            padding-top: 130px;
            padding-bottom: 60px;
        }
    }
</style>

