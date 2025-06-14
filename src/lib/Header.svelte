<script>
  import EmailLink from "./EmailLink.svelte";
  import Logo from "./Logo.svelte";
  import PhoneLink from "./PhoneLink.svelte";

  let { scrollPosition = 0, heigh = 0 } = $props();

  let gradientPos = $derived(Math.round((scrollPosition / heigh) * 300));

  let gradientSecondParam = $derived(Math.max(0, Math.min(100, gradientPos)));
</script>

<header
  class={`h-20 fixed top-0 text-[#f5d196] z-10 w-full`}
  data-gradient-pos={isNaN(gradientSecondParam) ? 0 : gradientSecondParam}
  style={`background: linear-gradient(to bottom, #271d1d 0%, #271d1d calc(${gradientSecondParam}%),transparent calc(${gradientSecondParam + 1}%), transparent 100%);`}
>
  <div
    class="h-full flex justify-between items-center max-w-7xl mx-auto py-4 px-6"
  >
    <Logo />
    <div class="shrink-1 grow-0 flex gap-8 text-4xl text-[#f5d196]">
      <PhoneLink animate />
      <EmailLink animate />
    </div>
  </div>
</header>

<style>
  header {
    transition: background-color 0.3s ease-in-out;
  }
</style>
