<section id="hero" class="d-flex home align-items-center">
    <div class="container text-center text-lg-start">
        <div class="row">
            <div class="col-sm-12 col-lg-7 hero-title d-flex justify-content-center">
                <h1 class="text-center">Aurélie <span>Millet</span></h1>
                <div class="btns text-center">
                    <a href="/presentation" class="btn-menu">Présention</a>
                    <a href="/contact" class="btn-book">Contact</a>
                </div>
            </div>

            <div class="round-img">
            </div>
        </div>
    </div>
</section>

<style lang="scss">
  @use '@unsass/breakpoint';

  .home {
    width: 100%;
    height: calc(100vh - 120px);
    position: relative;
    padding: 0;
    overflow: hidden;
  }

  /* Background Image with Overlay */
  .home::before {
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


  .home .container {
    padding-top: 110px;
  }

  @media (max-width: 992px) {
    .home .container {
      padding-top: 0;
    }
  }

  .home h1 {
    margin: 0;
    font-size: 64px;
    font-weight: 700;
    line-height: 56px;
    color: #fff;
  }

  .home h1 span {
    color: var(--secondary-color);
  }

  .home .btns {
    margin-top: 30px;
  }

  .home .btn-menu, .home .btn-book {
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

  .home .btn-menu:hover, .home .btn-book:hover {
    background: var(--secondary-color);
    color: #fff;
  }

  .home .hero-title {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  .home .round-img {
    height: 400px;
    width: 400px;
    border-radius: 50%;
    position: relative;
  }

  .home .round-img::before {
    content: '';
    position: absolute;
    border-radius: 50%;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    background-image: url('$lib/assets/profil.jpg');
    background-position: top;
    background-size: cover;
    z-index: 2;
  }

  .home .round-img::after {
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
    .home {
      background-attachment: fixed;
    }
  }

  @media (max-width: 992px) {
    .home {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
    }

    .home .row {
      flex-direction: column;
      align-items: center;
      justify-content: center;
      gap: 30px;
    }

    .home .round-img {
      margin-top: 100px;
      height: 300px;
      width: 300px;
    }
  }

  @media (max-height: 500px) {
    .home {
      height: auto;
    }
    .home .container {
      padding-top: 130px;
      padding-bottom: 60px;
    }
  }
</style>

