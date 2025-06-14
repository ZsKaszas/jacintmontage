<script>
  import SectionWrapper from "./SectionWrapper.svelte";
  import PhoneLink from "./PhoneLink.svelte";
  import EmailLink from "./EmailLink.svelte";
  import InstagramLink from "./InstagramLink.svelte";
  import FacebookLink from "./FacebookLink.svelte";
</script>

<footer class="bg-[#271d1d] text-[#f5d196]">
  <SectionWrapper>
    <div
      class="grid grid-cols-2 sm:grid-cols-3 justify-between gap-4 items-center text-center"
    >
      <div class="col-span-2 sm:col-span-1"></div>
      <div class="text-2xl">Seit 2024</div>
      <div class="flex gap-2 sm:gap-8 text-2xl justify-center sm:justify-end">
        <PhoneLink />
        <EmailLink />
        <FacebookLink />
        <InstagramLink />
      </div>
    </div>
  </SectionWrapper>
</footer>
