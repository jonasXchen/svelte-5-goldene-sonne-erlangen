<script>
  import Header from "../pages/Header.svelte";
  import Food from "../pages/Food.svelte";
  import Facilities from "../pages/Facilities.svelte";
  import Directions from "../pages/Directions.svelte";
  import Footer from "../pages/Footer.svelte";
  import {
    PUBLIC_RESTAURANT_CITY,
    PUBLIC_RESTAURANT_NAME,
  } from "$lib/constants";
</script>

<svelte:head>
  <!-- Basic Meta Tags -->
  <meta name="{PUBLIC_RESTAURANT_NAME} {PUBLIC_RESTAURANT_CITY}" content="" />
  <meta
    name="keywords"
    content="{PUBLIC_RESTAURANT_NAME}, {PUBLIC_RESTAURANT_CITY}"
  />
  <link rel="icon" href="/logo.png" />
  <title>{PUBLIC_RESTAURANT_NAME}</title>
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
