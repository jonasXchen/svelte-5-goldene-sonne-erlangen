<script>
  import BuffetImage from "/src/assets/images/Food2.png";
  import CustomWhiteImage from "/src/assets/images/custom-white-bg.png";
  import DessertImage from "/src/assets/images/Food5.png";
  import Menu from "/src/assets/menu/2024-10-10_Speisekarte.pdf";
</script>

<div class="flex flex-col w-full gap-8 p-8 bg-white lg:px-8 md:px-20 sm:px-16">
  <div class="flex flex-col items-center w-full gap-8 h-4/5 lg:flex-row">
    <!-- Buffet -->
    <div class="flex flex-col items-center w-full lg:w-1/2 lg:relative">
      <img
        src={BuffetImage}
        alt="Buffet Image"
        class="lg:z-30 lg:absolute lg:-right-20 lg:transform lg:-translate-y-1/2 object-cover min-h-60 w-full lg:w-fit h-[380px] md:max-h-[400px] max-h-[240px] sm:max-h-[320px]"
      />
    </div>
    <div
      class="flex lg:w-1/2 flex-col lg:gap-2 lg:h-[500px] justify-center max-h-[500px] relative sm:p-12 p-8 w-full"
      style="background-image: url('{CustomWhiteImage}');"
    >
      <div class="flex flex-col gap-4 lg:z-20 lg:p-16 lg:left-10 lg:absolute">
        <div
          class="text-3xl font-medium tracking-widest font-cinzel text-primary"
        >
          Speisen
        </div>
        <p class="text-xl font-semibold">Jeder Geschmack is dabei!</p>
        <p class="text-balance">
          Nutzen Sie die Gelegenheit und genießen Sie unser zahlreiches
          Speisenangebot!
        </p>
        <a href={Menu} target="_blank" rel="noopener noreferrer">
          <button
            class="w-full p-2 font-semibold bg-white border-2 border-primary text-primary max-w-64"
            >Zur Hauptspeisekarte
          </button>
        </a>
      </div>
    </div>
  </div>

  <!-- Desserts -->
  <div class="flex flex-col items-center w-full gap-8 h-4/5 lg:flex-row">
    <div
      class="flex flex-col items-center w-full lg:w-1/2 lg:relative lg:order-2"
    >
      <img
        src={DessertImage}
        alt="Buffet Image"
        class="lg:z-30 lg:absolute lg:-left-20 lg:transform lg:-translate-y-1/2 object-cover min-h-60 w-full lg:w-fit h-[380px] md:max-h-[400px] max-h-[240px] sm:max-h-[320px]"
      />
    </div>
    <div
      class="flex lg:w-1/2 flex-col lg:gap-2 lg:h-[500px] lg:max-h-[500px] justify-center relative sm:p-12 p-8 w-full"
      style="background-image: url('{CustomWhiteImage}');"
    >
      <div class="flex flex-col gap-4 lg:z-20 lg:p-16 lg:right-10 lg:absolute">
        <div
          class="text-3xl font-medium tracking-widest font-cinzel text-primary"
        >
          Traditionelle Gerichte
        </div>
        <p class="text-xl font-semibold">Umfangreich und lecker!</p>
        <p class="text-balance">
          Von allen Köstlichkeiten etwas dabei, wählen Sie Ihre Wunschnachspeise
          aus!
        </p>
        <a href={Menu} target="_blank" rel="noopener noreferrer">
          <button
            class="w-full p-2 font-semibold bg-white border-2 border-primary text-primary max-w-64"
            >Zur traditionellen Speisekarte</button
          >
        </a>
      </div>
    </div>
  </div>
</div>
