<script>
  import {
    PUBLIC_ENTITY_LUNCH_TIME,
    PUBLIC_ENTITY_DINNER_TIME,
    PUBLIC_ENTITY_OPENING_DAYS,
  } from "$lib/constants";

  import DirectionsImage from "/src/assets/images/directions.png";
</script>

<div class="flex flex-col w-full gap-8 p-8 lg:px-8 md:px-20 sm:px-16">
  <div class="flex w-full">
    <p
      class="w-full text-3xl font-medium tracking-widest text-center font-cinzel text-primary sm:text-left"
    >
      So finden Sie uns!
    </p>
  </div>
  <p class="text-center text-balance sm:text-left">
    <span class="font-bold">{PUBLIC_ENTITY_OPENING_DAYS}</span>, auch an
    <span class="font-bold">Feiertagen</span>
    ab
    <span class="font-bold">{PUBLIC_ENTITY_LUNCH_TIME}</span> &
    <span class="font-bold">{PUBLIC_ENTITY_DINNER_TIME}</span> sind wir für Sie da!
  </p>
  <div class="flex flex-col gap-8 lg:flex-row lg:gap-12">
    <div class="flex flex-col w-full gap-4">
      <!-- Map -->
      <div class="flex w-full sm:h-[320px] md:h-[400px] h-[240px]">
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d10345.265272991406!2d11.0051418!3d49.5917841!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47a1f9c1c206c3f3%3A0x5aa647340fbc428b!2sChina%20Restaurant%20Goldene%20Sonne!5e0!3m2!1sde!2ssg!4v1725606987201!5m2!1sde!2ssg"
          width="100%"
          height="100%"
          style="border:0;"
          allowfullscreen=""
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"
        ></iframe>
      </div>
    </div>
    <div class="flex flex-col w-full gap-4">
      <img
        src={DirectionsImage}
        class="md:h-[360px] sm:h-[280px] object-cover h-[200px] w-full"
      />
      <p class="text-center text-balance sm:text-left">
        Auch mit Baustelle, ausreichend Parkplätze direkt unter dem
        Einkaufszentrum und Restaurant.
      </p>
    </div>
  </div>
</div>
