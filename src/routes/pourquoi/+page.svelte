<script>
    import { HeartHandshake, Users, MoveRight } from 'lucide-svelte';
</script>

<div class="section-title p-5">
    <h2>

        Pourquoi ? Pour qui ?
    </h2>
    <p>Les explications</p>
</div>

<section class="pourquoi p-5">


    <div class="content-section">
        <div class="content-block">
            <h3>
                <HeartHandshake/>
                Pourquoi consulter?
            </h3>
            <p>Franchir le pas pour consulter un psychologue n'est pas toujours facile à réaliser. Au cours d'une vie,
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
                Pour qui?
            </h3>
            <p>Je peux accueillir toute personne qui en fait la demande. N'hésitez pas à me contacter afin que l'on
                puisse échanger sur votre demande et vos besoins.</p>
            <ul class="mb-3">
                <li>
                    <MoveRight class="me-2"/>
                    Enfants, Adolescents, Adultes
                </li>
                <li>
                    <MoveRight class="me-2"/>
                    Aidants naturels
                </li>
                <li>
                    <MoveRight class="me-2"/>
                    Personnes âgées ou souffrant d’une pathologie invalidante
                </li>
            </ul>
            <p>Frais supplémentaires de déplacement : 5€</p>
        </div>
    </div>
</section>

<style lang="scss">
  .pourquoi {
    background-color: var(--primary-color-lighter);
    color: var(--white-color);
    padding: 20px;

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
