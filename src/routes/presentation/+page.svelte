<script>
    import img from '$lib/assets/lily.webp';
    import { Award, GraduationCap } from 'lucide-svelte';
</script>

<section id="presentation" class="presentation hero p-5">
    <div class="upper-section">
        <div class="left-section">
            <div class="section-title">
                <h2>Présentation</h2>
                <p>En quelques mots</p>
            </div>
            <p>
                <strong style="color: var(--secondary-color);">Psychologue clinicienne, Praticienne EFT & Conseillère en produits de soins naturels</strong>
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
        </div>
        <div class="right-section">
            <img src="{img}" alt="Portrait of Aurélie, the clinician"/>
        </div>
    </div>
    <div class="lower-section">
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
        <h2 class="my-4"><i class="bi bi-card-list"></i> <GraduationCap /> Diplômes</h2>
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


  #presentation {
    text-align: justify;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    .upper-section {
      display: flex;
      flex-wrap: wrap;
    }
    .left-section {
      max-width: 730px;
    }


    .left-section, .right-section {
      flex: 1;
      padding: 20px;
    }

    .right-section {
      display: flex;
      justify-content: flex-start;
      align-items: center;

      img {
        border-radius: 12px;
        object-fit: cover;
        width: 100%;
        max-width: 500px;
        max-height: 500px;
      }
    }

    .lower-section {
      padding: 20px;
      width: 100%;
      max-width: 1100px;
    }

    h2 {
      color: var(--secondary-color);
    }

  }

  @media (min-width: 601px) and (max-width: 1024px) {
    #presentation .upper-section {
      flex-direction: row;
    }
  }

  @media (max-width: 800px) {
    #presentation {
      .upper-section {
        flex-direction: column;
      }

      .left-section, .right-section, .lower-section {
        padding: 10px;
      }

      .right-section img {
        max-width: 100%;
        max-height: none;
      }
    }
  }
</style>
