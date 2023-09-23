<script>
    import 'bootstrap/dist/css/bootstrap.min.css';
    import '../styles/main.scss';
    import Header from "$lib/components/Header.svelte";
    import 'leaflet/dist/leaflet.css';
</script>

<!-- Header -->
<Header/>

<!-- Main content-->
<slot/>
