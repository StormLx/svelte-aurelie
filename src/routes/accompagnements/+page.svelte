<script>
    import { BookMarked, Leaf, Cross, AlertTriangle } from 'lucide-svelte';
</script>

<div class="section-title p-5">
    <h2 data-aos="slide-right">
        Mes accompagnements
    </h2>
    <p>En détail</p>
</div>

<section id="accompagnements" class="accompagnement p-5">

    <div class="content-section">
        <div class="content-block">
            <h3>
                <BookMarked/>
                Consultations de soutien psychologique
            </h3>
            <p>Mon approche est intégrative, s’appuyant sur différents courants pour tenir compte de la complexité de
                l’être humain.</p>
            <p>En évaluant ensemble votre demande, nous établirons s’il s’agit d’un accompagnement psychologique de
                soutien ponctuel ou d’un accompagnement psychothérapeutique plus long.</p>
        </div>

        <div class="content-block">
            <h3>
                <Leaf/>
                Séances d'EFT Clinique
            </h3>
            <p>L’EFT (Emotionnal Freedom Technique) est une pratique psychocorporelle visant à traiter des blocages
                émotionnels. Les principes de l’EFT s’appuient sur les fondements des thérapies traditionnelles et
                ancestrales en
                alliant psychologie et acupuncture.</p>
            <details>
                <summary>Lire plus</summary>
                <p>
                    Cette technique qui s’attache au lien entre le corps et l’esprit permet d’apporter un soulagement
                    émotionnel rapide et durable en traitant la cause de l’émotion négative. Selon le fondateur, Gary
                    Craig, toutes les émotions négatives sont provoquées par une perturbation de l’équilibre énergétique
                    du corps. En effet, notre corps serait parcouru par des circuits énergétiques qui peuvent être
                    fortement perturbés lorsqu’un choc émotionnel survient. Cela va donner lieu à des émotions
                    négatives qui peuvent être supprimées en rétablissant l’équilibre énergétique du corps.
                </p>
                <p>
                    Ce rééquilibrage se fait en tapotant du bout des doigts les extrémités de certains méridiens
                    énergétiques issus de l’acupuncture, ce qui va permettre de refaire circuler l’énergie normalement.
                    Cela contribuerait à réduire la charge émotionnelle associée à un souvenir traumatique, et à changer
                    l’attitude de l’individu face à son problème.
                </p>
            </details>
        </div>

        <div class="content-block">
            <h3>
                <Cross/>
                Conseils en produits de soins naturels
            </h3>
            <p>
                La phytothérapie, l'aromathérapie ainsi que les produits de la ruche peuvent être un complément aux
                thérapies psychologiques et énergétiques.
            </p>
            <p>
                Lors d'une séance, si le contexte ou une situation le permet et surtout si cela fait sens pour vous,
                je peux vous proposer des conseils en produits de soins naturels afin de venir compléter le travail
                effectué ensemble.
            </p>

            <details>
                <summary>Lire plus</summary>
                <p>
                    <strong>La phytothérapie</strong>, étymologiquement le traitement par les plantes, est une méthode
                    thérapeutique
                    qui utilise l’action des plantes médicinales. Elle fait partie des médecines ancestrale que l'on
                    utilise
                    depuis des siècles sous forme de tisanes et plus récemment sous forme d'extrait sec en gélule.
                </p>

                <p><strong>La gemmothérapie</strong> est une branche de la phytothérapie. Elle s’en distingue néanmoins
                    par l’usage,
                    non plus d’un élément de la plante adulte (feuille, écorce, tige, racine, fleur), mais de sa partie
                    embryonnaire (bourgeon, jeunes pousses, radicelles).
                </p>
                <p>Son utilisation permet d’obtenir des thérapeutiques plus actives, il n’est donc pas nécessaire de
                    prendre des doses importantes.</p>
                <p><strong>L'aromathérapie</strong> est une approche de soin qui utilise les extraits aromatiques des
                    plantes, comme
                    les huiles essentielles, les huiles végétales ou des extraits de plante à des fins thérapeutiques ou
                    de
                    bien-être</p>
                <p>L'aromathérapie peut apporter une aide pour traiter certains troubles mineurs comme le stress, la
                    fatigue, les problèmes de peau, les migraines ou les douleurs articulaires ou musculaires, la
                    digestion...
                </p>
                <p>Régulatrice à la fois du système neuronal et hormonal, elle agit en profondeur sur le rééquilibrage
                    de
                    l'organisme de part ses molécules bio-chimiques.
                </p>
                <p>Une huile essentielle bien choisie et bien utilisée pourra aider au lâcher prise et à la détente.</p>
                <p>Certaines sont apaisantes et relaxantes, pendant que d'autres sont davantage stimulantes et
                    énergisantes.</p>
                <p>Leur utilisation est puissante et il est nécessaire de les utiliser avec précaution, c'est pourquoi
                    j'ai suivi
                    la formation de conseillère en produits de soins naturels pour vous conseiller au mieux. </p>
                <p><strong>L'apithérapie</strong> est une thérapeutique douce qui utilise les produits de la ruche,
                    principalement
                    le miel,
                    la propolis, la gelée royale et le pollen à des fins thérapeutiques ou préventives.</p>
                <p>L'apithérapie est reconnue et utilisée depuis des milliers d'années dans de nombreuses cultures à
                    travers le monde pour ses différentes vertus et bienfaits.</p>
                <p>Les produits issus de l'apiculture sont réputés pour leurs propriétés anti-inflammatoires,
                    antimicrobiennes, cicatrisantes, antioxydantes...</p>
                <p>Ils contiennent divers composés bioactifs comme des vitamines, des minéraux, des enzymes ou des
                    acides aminés qui ont un effet positif sur la santé humaine en soutenant et renforçant
                    l'organisme. </p>
            </details>


        </div>

    </div>

    <p class="disclaimer">
        <AlertTriangle/>
        Toutefois, toutes ces thérapies que l'on peut attribuer aux médecines douces et naturelles ne
        prétendent pas se substituer à la médecine conventionnelle.
    </p>
</section>

<style lang="scss">
  .accompagnement {
    text-align: justify;
    padding: 20px;
    background-color: var(--primary-color-lighter);
    color: var(--white-color);

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
</style>
