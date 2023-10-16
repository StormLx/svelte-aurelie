<script>
    import 'bootstrap/dist/css/bootstrap.min.css';
    import '../styles/main.scss';
    import Header from "$lib/components/Header.svelte";
    import 'leaflet/dist/leaflet.css';
    import Footer from "$lib/components/Footer.svelte";
</script>

<svelte:head>
    <title>Aurélie Millet Psychologue Clinicienne</title>
    <meta name="google-site-verification" content="7Q5IzLVJUG6w_3lSr6f9vlWmpPzCL0AV35D0nHQH8M8" />
    <meta name="description" content="Psychologue clinicienne, je vous accueille dans mon cabinet pour des consultations individuelles, familiales ou de couple.">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</svelte:head>

<!-- Header -->
<Header/>

<!-- Main content-->
<slot/>

<!-- Footer -->
<Footer/>
