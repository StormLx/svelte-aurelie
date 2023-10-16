<script>
    import { BookMarked, Leaf, Cross, AlertTriangle } from 'lucide-svelte';
    import eft from '$lib/assets/eft.jpg';
    import soin from '$lib/assets/soin-naturel.jpg';
    import soutien from '$lib/assets/soutien.png';
</script>


<section id="accompagnements" class="hero accompagnement p-5">

    <div class="content">
        <div class="section-title">
            <h2 data-aos="slide-right">
                Mes accompagnements
            </h2>
            <p>En détail</p>
        </div>

        <div class="content-section">
            <div class="content-block d-flex justify-content-center align-items-center gap-5">
                <div class="side--text">
                    <h3>
                        <BookMarked/>
                        Consultations de soutien psychologique
                    </h3>
                    <p>Mon approche est intégrative, s’appuyant sur différents courants pour tenir compte de la
                        complexité
                        de
                        l’être humain.</p>
                    <p>En évaluant ensemble votre demande, nous établirons s’il s’agit d’un accompagnement psychologique
                        de
                        soutien ponctuel ou d’un accompagnement psychothérapeutique plus long.</p></div>
                <div class="round-img soutien"></div>
            </div>

            <div class="content-block d-flex justify-content-center align-items-center gap-5">
                <div>
                    <h3>
                        <Leaf/>
                        Séances d'EFT Clinique
                    </h3>
                    <p>L’EFT (Emotionnal Freedom Technique) est une pratique psychocorporelle visant à traiter des
                        blocages
                        émotionnels. Les principes de l’EFT s’appuient sur les fondements des thérapies traditionnelles
                        et
                        ancestrales en
                        alliant psychologie et acupuncture.</p>
                    <details>
                        <summary>Lire plus</summary>
                        <p>
                            Cette technique qui s’attache au lien entre le corps et l’esprit permet d’apporter un
                            soulagement
                            émotionnel rapide et durable en traitant la cause de l’émotion négative. Selon le fondateur,
                            Gary
                            Craig, toutes les émotions négatives sont provoquées par une perturbation de l’équilibre
                            énergétique
                            du corps. En effet, notre corps serait parcouru par des circuits énergétiques qui peuvent
                            être
                            fortement perturbés lorsqu’un choc émotionnel survient. Cela va donner lieu à des émotions
                            négatives qui peuvent être supprimées en rétablissant l’équilibre énergétique du corps.
                        </p>
                        <p>
                            Ce rééquilibrage se fait en tapotant du bout des doigts les extrémités de certains méridiens
                            énergétiques issus de l’acupuncture, ce qui va permettre de refaire circuler l’énergie
                            normalement.
                            Cela contribuerait à réduire la charge émotionnelle associée à un souvenir traumatique, et à
                            changer
                            l’attitude de l’individu face à son problème.
                        </p>
                    </details>
                </div>

                <div class="round-img eft"></div>

            </div>

            <div class="content-block d-flex justify-content-center align-items-center gap-5">
                <div>
                    <h3>
                        <Cross/>
                        Conseils en produits de soins naturels
                    </h3>
                    <p>
                        La phytothérapie et l'aromathérapie peuvent être un complément aux
                        thérapies psychologiques et énergétiques.
                    </p>
                    <p>
                        Lors d'une séance, si le contexte ou une situation le permet et surtout si cela fait sens pour
                        vous,
                        je peux vous proposer des conseils en produits de soins naturels afin de venir compléter le
                        travail
                        effectué ensemble.
                    </p></div>

                <div class="round-img soins"></div>
            </div>

        </div>

        <p class="disclaimer">
            <AlertTriangle/>
            Toutefois, toutes ces thérapies que l'on peut attribuer aux médecines douces et naturelles ne
            prétendent pas se substituer à la médecine conventionnelle. En aucun cas mes conseils n'iront à l'encontre
            d'un avis médical.
        </p>
    </div>
</section>

<style lang="scss">
  @use '@unsass/breakpoint';

  .accompagnement {
    text-align: justify;
    @include breakpoint.down('md') {
      padding: 20px !important;
    }
    color: var(--white-color);
    margin: auto;

    .content {
      width: 70%;
      margin: 0 auto;
      @include breakpoint.down('md') {
        width: 100%;
      }
    }

    .section-title {
      h2 {
        display: flex;
        align-items: center;
        gap: 10px;
        color: var(--secondary-color);
      }
    }

    .content-section {
      .content-block {
        margin-bottom: 20px;

        h3 {
          display: flex;
          align-items: center;
          gap: 10px;
          color: var(--secondary-color);
        }

        details {
          margin-top: 10px;

          summary {
            margin-bottom: 10px;
          }
        }
      }
    }

    .disclaimer {
      color: lightcoral;
      margin-top: 20px;
    }
  }

  .round-img {
    height: 300px;
    width: 600px;
    border-radius: 50%;
    background-size: cover;
    background-position: center;
  }

  .soutien {
    background-image: url("$lib/assets/soutien.png");
  }

  .eft {
    background-image: url("$lib/assets/eft.jpg");
  }

  .soins {
    background-image: url("$lib/assets/soin-naturel.jpg");
  }
</style>
