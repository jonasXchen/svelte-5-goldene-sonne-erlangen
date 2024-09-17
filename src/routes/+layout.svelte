<script>
  // Injecting TailwindCss
  import "../app.css";

  // Injecting Vercel Analytics
  import { dev } from "$app/environment";
  import { inject } from "@vercel/analytics";
  import DeclarationOfConsent from "../components/DeclarationOfConsent.svelte";

  inject({ mode: dev ? "development" : "production" });
</script>

<main class="text-base font-light font-overpass md:text-lg">
  <slot />
  <DeclarationOfConsent
    popupClass="bg-white"
    acceptClass="bg-primary text-white"
  />
</main>
