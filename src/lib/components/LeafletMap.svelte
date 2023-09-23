<script>
    import { onMount, onDestroy } from 'svelte';
    import { browser } from '$app/environment';

    let mapElement;
    let map;

    onMount(async () => {
        if(browser) {
            const leaflet = await import('leaflet');
            const lat = 44.1179562;
            const long = 4.9006627;

            map = leaflet.map(mapElement).setView([lat, long], 20.25);

            leaflet.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
                attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
            }).addTo(map);

            leaflet.marker([lat, long]).addTo(map)
                .bindPopup('Aurélie Millet<br>Pôle Sante Via Venaissia.<br> 29, Av. du Onze Novembre, 84150 Jonquières.<br> ')
                .openPopup();
        }
    });

    onDestroy(async () => {
        if(map) {
            console.log('Unloading Leaflet map.');
            map.remove();
        }
    });
</script>


<main>
    <div bind:this={mapElement}></div>
</main>

<style lang="scss">
    main div {
        height: 400px;
    }
</style>
