<script>
  let {
    popupClass = "",
    acceptClass = "",
    declineClass = "",
    detailsHref = "/datenschutz",
    onAccept = () => {},
    onDecline = () => {},
  } = $props();

  let showPopup = $state(true);

  const acceptCookies = () => {
    onAccept();
    showPopup = false;
  };

  const declineCookies = () => {
    onDecline();
    showPopup = false;
  };
</script>

{#if showPopup}
  <div
    class="fixed bottom-0 left-0 right-0 z-50 gap-8 p-4 bg-black bg-opacity-50 backdrop-blur-md {popupClass}"
  >
    <div class="flex flex-col gap-2 p-4">
      <p class="text-xl font-bold">Declaration of Consent</p>
      <p>
        We use cookies and similar technologies to ensure that you have the best
        possible experience on our website. Please confirm your consent to use
        these technologies.
      </p>
      <a class="text-sm font-thin underline" href={detailsHref}>
        <p>Read about details -></p>
      </a>

      <div class="flex flex-row self-end gap-4">
        <button
          on:click={acceptCookies}
          class="p-2 text-white border border-white bg-priamry {acceptClass}"
          >Accept</button
        >
        <button
          on:click={declineCookies}
          class="p-2 text-black bg-gray-300 {declineClass}">Decline</button
        >
      </div>
    </div>
  </div>
{/if}
