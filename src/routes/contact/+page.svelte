<script>
    import { Phone, Mail, MapPin, Clock10, Euro } from 'lucide-svelte';
    import LeafletMap from '$lib/components/LeafletMap.svelte';


</script>

<section class="hero page-section p-5">
    <div class="section-title">
        <h2>Les séances</h2>
    </div>


    <div class="card">
        <h3>
            <Clock10/>
            Durée
        </h3>
        <p>45 min à 1h</p>
    </div>

    <div class="card">
        <h3>
            <Euro/>
            Tarifs
        </h3>
        <p>En cabinet: 50€</p>
        <p>À domicile: 55€</p>
    </div>

    <div class="card">
        <h3>Informations pratiques</h3>
        <p>Modalités de paiement: Le règlement s’effectue par chèque ou en espèces en fin de séance.</p>
        <p>Les entretiens ne sont pas remboursés par la Sécurité Sociale, néanmoins certaines mutuelles proposent des
            remboursements. Renseignez-vous auprès de votre mutuelle santé.</p>
        <p>Une facture peut être éditée à la demande.</p>
    </div>

    <div class="section-title mt-5">
        <h2>Contact</h2>
    </div>

    <div class="card">
        <h3>
            <Phone/>
            Pour prendre RDV
        </h3>

        <p>Ouverture du cabinet :</p>
        <ul>
            <li>Lundi 14h-18h30</li>
            <li>Jeudi 9h-18h</li>
        </ul>
        <br>
        <p>Par téléphone: 07 81 04 28 18</p>
        <p>
            <Mail/>
            Par e-mail: <a href="mailto:amillet.psychologue@gmail.com?subject=Prise de rendez-vous">amillet.psychologue@gmail.com</a>
        </p>
    </div>

    <div class="card">
        <h3>
            <MapPin/>
            Pour me localiser
        </h3>
        <p>Pôle Sante Via Venaissia</p>
        <p>29, Av. du Onze Novembre, 84150 Jonquières</p>
        <LeafletMap/>
    </div>
</section>

<style lang="scss">

  @use '@unsass/breakpoint';

  .page-section {
    color: var(--white-color);
    @include breakpoint.down('md') {
      padding: 20px !important;
    }
    height: auto;


    .section-title {
      width: 70%;
      margin: 10px auto;

      h2 {
        color: var(--secondary-color);
        font-size: 2rem;
        margin-bottom: 10px;
      }

      p {
        font-size: 1.25rem;
        margin-bottom: 20px;
      }

      @include breakpoint.down('md') {
        width: 100%;
      }
    }

    .card {
      background-color: var(--primary-color-lighter);
      color: var(--white-color);
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
      width: 70%;
      margin: 10px auto;
      @include breakpoint.down('md') {
        width: 100%;
      }

      h3 {
        display: flex;
        align-items: center;
        gap: 10px;
        color: var(--secondary-color);
        font-size: 1.5rem;
        margin-bottom: 10px;
      }

      p {
        margin-bottom: 10px;
      }
    }
  }
</style>
