<script>
  import Header from "../pages/Header.svelte";
  import Food from "../pages/Food.svelte";
  import Facilities from "../pages/Facilities.svelte";
  import Directions from "../pages/Directions.svelte";
  import Footer from "../pages/Footer.svelte";
  import { PUBLIC_ENTITY_CITY, PUBLIC_ENTITY_NAME } from "$lib/constants";
</script>

<svelte:head>
  <!-- Basic Meta Tags -->
  <meta name="{PUBLIC_ENTITY_NAME} {PUBLIC_ENTITY_CITY}" content="" />
  <meta name="keywords" content="{PUBLIC_ENTITY_NAME}, {PUBLIC_ENTITY_CITY}" />
  <link rel="icon" href="/logo.png" />
  <title>{PUBLIC_ENTITY_NAME}</title>
</svelte:head>

<div class="flex flex-col items-center">
  <Header />
  <div class="flex flex-col max-w-[1080px]">
    <Food />
    <Facilities />
    <Directions />
  </div>
  <Footer />
</div>
