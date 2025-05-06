<script>
  import SectionWrapper from "./SectionWrapper.svelte";
  import Logo from "./Logo.svelte";
</script>

<footer class="bg-[#271d1d] text-[#f5d196]">
  <SectionWrapper>
    <div
      class="grid grid-cols-2 sm:grid-cols-3 justify-between gap-4 items-center text-center"
    >
      <div
        class="h-20 col-span-2 sm:col-span-1 flex justify-center items-center"
      >
        <Logo />
      </div>
      <div class="text-2xl">Seit 2024</div>
      <div class="flex gap-4 text-2xl justify-end">
        <span class="icon-[line-md--facebook]"></span>
        <span class="icon-[line-md--instagram]"></span>
      </div>
    </div>
  </SectionWrapper>
</footer>
