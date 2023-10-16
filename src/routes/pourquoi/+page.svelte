<script>
    import { HeartHandshake, Users, MoveRight } from 'lucide-svelte';
</script>


<section class="pourquoi hero p-5">
    <div class="content">

        <div class="section-title">
            <h2>
                Pour quoi ? Pour qui ?
            </h2>
            <p>Les explications</p>
        </div>


        <div class="content-section">
            <div class="content-block">
                <h3>
                    <HeartHandshake/>
                    Pourquoi consulter ?
                </h3>
                <p>Franchir le pas pour consulter un psychologue n'est pas toujours facile à réaliser. Au cours d'une
                    vie,
                    il existe de nombreuses raisons de rencontrer un psychologue...</p>
                <ul class="mb-3">
                    <li>
                        <MoveRight class="me-2"/>
                        Gestion émotionnelle
                    </li>
                    <li>
                        <MoveRight class="me-2"/>
                        Conflits familiaux ou relationnels
                    </li>
                    <li>
                        <MoveRight class="me-2"/>
                        Maladies, deuils, séparations
                    </li>
                    <li>
                        <MoveRight class="me-2"/>
                        Stress, anxiété, dépression
                    </li>
                </ul>
                <p>Et cela concerne tous les âges de la vie.</p>
            </div>

            <div class="content-block">
                <h3>
                    <Users/>
                    Pour qui ?
                </h3>
                <p>Je peux accueillir toute personne qui en fait la demande.</p>
                <ul class="mb-3">
                    <li>
                        <MoveRight class="me-2"/>
                        Enfants, Adolescents, Adultes
                    </li>
                    <li>
                        <MoveRight class="me-2"/>
                        Personnes âgées ou souffrant d’une pathologie invalidante
                    </li>
                    <li>
                        <MoveRight class="me-2"/>
                        Aidants naturels
                    </li>
                </ul>
                <p>Je suis en mesure de me déplacer pour des consultations dans un périmètre de 7 kilomètres. <br>
                    Je vous invite à me contacter afin de discuter en détail de vos besoins et attentes. <br>
                    Veuillez noter qu'un supplément tarifaire de 5€ est applicable.</p>
            </div>
        </div>
    </div>
</section>

<style lang="scss">
  @use '@unsass/breakpoint';


  .pourquoi {
    color: var(--white-color);
    @include breakpoint.down('md') {
      padding: 20px !important;
    }

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

        ul {
          padding-left: 20px;
        }
      }
    }
  }
</style>
