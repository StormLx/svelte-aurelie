<script>
    import { Award, GraduationCap } from 'lucide-svelte';
</script>

<section id="presentation" class="hero presentation p-5">
    <div class="content">

        <div class="section-title">
            <h2>Présentation</h2>
            <p>En quelques mots</p>
        </div>
        <p>
            <strong style="color: var(--secondary-color);">Psychologue clinicienne, Praticienne EFT & Conseillère en
                produits de soins naturels</strong>
            <br><br>
            Issue de l’Université Toulouse II, j'ai initialement orienté ma pratique clinique vers la psychologie
            clinique du vieillissement et la neuropsychologie. Ma curiosité professionnelle m’a amenée à explorer
            les
            troubles psychologiques associés au vieillissement, qu'il soit optimal ou pathologique.
        </p>
        <p>
            <i class="bi bi-journal-medical"></i> Mes expériences variées et mes formations complémentaires m'ont
            ensuite guidée vers le domaine de l'oncologie et des soins palliatifs. Cette immersion m’a confrontée à
            des
            questionnements profonds, enrichissant ma pratique et m'incitant à envisager d'autres approches pour mes
            séances.
        </p>


        <p>
            <i class="bi bi-heart-half"></i> Mon approche clinique se base sur une rencontre présente, centrée sur l’ici
            et maintenant. Je suis là pour vous guider dans votre parcours de vie, en valorisant les ressources
            intérieures que vous possédez déjà. Mon objectif est de renforcer votre autonomie psychique et de vous aider
            à redevenir maître de votre vie.
        </p>
        <p>
            <i class="bi bi-patch-check-fill"></i> Outre un soutien psychologique traditionnel, j’offre, lorsque la
            situation s’y prête, des sessions de thérapies brèves de libération émotionnelle (EFT).
        </p>
        <p>
            <i class="boxicons bx bxs-leaf"></i> Animée par une passion pour la nature et ses bienfaits, je me suis
            également formée en tant que conseillère en produits de soins naturels. Cette compétence complémentaire me
            permet de vous suggérer des solutions naturelles pour des problématiques courantes telles que l'anxiété, le
            stress ou les troubles du sommeil...
        </p>
        <h2 class="my-4"><i class="bi bi-card-list"></i>
            <GraduationCap/>
            Diplômes
        </h2>
        <ul>
            <li>
                <Award style="color: var(--secondary-color);"/>
                2023: Certification EFT (Emotional Freedom Technique)
            </li>
            <li>
                <Award style="color: var(--secondary-color);"/>
                2022: Certification de Conseiller en Produits de Soins Naturels
            </li>
            <li>
                <Award style="color: var(--secondary-color);"/>
                2016: DU de Soins Palliatifs
            </li>
            <li>
                <Award style="color: var(--secondary-color);"/>
                2013: Master de Psychologie clinique et Gérontologie
            </li>
            <li>
                <Award style="color: var(--secondary-color);"/>
                2012: DU de Neuropsychologie
            </li>
        </ul>
    </div>
</section>

<style lang="scss">
  @use '@unsass/breakpoint';

  #presentation {
    text-align: justify;
    @include breakpoint.down('md') {
      padding: 20px !important;
    }
    color: var(--white-color);
    margin: auto;

    h2 {
      color: var(--secondary-color);
    }

    .content {
      width: 70%;
      margin: 0 auto;
      @include breakpoint.down('md') {
        width: 100%;
      }
    }

  }

  @media (max-width: 1224px) {
    #presentation {
      padding: 50px 100px;
    }
  }

  @media (max-width: 768px) {
    #presentation {
      padding: 50px 20px;
    }
  }


</style>
