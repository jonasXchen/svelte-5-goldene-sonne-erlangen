<script>
  import ImageCarousel from "../components/ImageCarousel.svelte";

  import EntranceImage from "/src/assets/images/entrance.png";
  import Facilities2Image from "/src/assets/images/facilities2.png";
  import Faciltiies3Image from "/src/assets/images/facilities3.png";
  import Facilities4Image from "/src/assets/images/facilities4.png";
  import Facilities5Image from "/src/assets/images/facilities5.png";

  let images = [
    {
      file: EntranceImage,
      name: "Herzlich Willkommen!",
    },
    {
      file: Facilities2Image,
      name: "Elegant traditionell",
    },
    {
      file: Faciltiies3Image,
      name: "Gemeinsam und gemütlich",
    },
    {
      file: Facilities4Image,
      name: "Schöner Ausblick",
    },
    {
      file: Facilities5Image,
      name: "Viel Platz",
    },
  ];
</script>

<div class="flex flex-col gap-8 p-8 lg:px-8 md:px-20 sm:px-16">
  <!-- Title -->
  <div
    class="flex text-3xl font-medium leading-10 tracking-widest font-cinzel text-primary"
  >
    Unsere Räumlichkeiten
  </div>
  <!-- Fotos -->
  <div class="relative flex">
    <!-- <div
      class="absolute top-0 left-0 bg-white [clip-path:polygon(0%_0%,100%_0%,100%_60%,0%_30%)] w-full h-1/5 opacity-35 z-20"
    ></div>
    <div
      class="absolute top-0 left-0 bg-white [clip-path:polygon(0%_0%,100%_0%,100%_60%,0%_30%)] w-full h-1/6 opacity-100 z-20"
    ></div> -->
    <ImageCarousel
      carouselClass="sm:h-[340px] lg:h-[640px] md:h-[440px] h-[280px] max-h-[620px] rounded-xl gap-0"
      imageClass="object-cover rounded-xl"
      imageTitle={true}
      {images}
    />
    <!-- <div
      class="absolute bottom-0 left-0 bg-white [clip-path:polygon(0%_0%,100%_50%,100%_100%,0%_100%)] w-full h-1/5 opacity-35"
    ></div>
    <div
      class="absolute bottom-0 left-0 bg-white [clip-path:polygon(0%_0%,100%_50%,100%_100%,0%_100%)] w-full h-1/6 opacity-100"
    ></div> -->
  </div>
</div>
