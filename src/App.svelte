<script>
  import Header from "./lib/Header.svelte";
  import SectionWrapper from "./lib/SectionWrapper.svelte";
  import Projects from "./lib/Projects.svelte";
  import WorkDetails from "./lib/WorkDetails.svelte";
  import Footer from "./lib/Footer.svelte";
</script>

<div class="main-bg">
  <main class="" id="main">
    <Header />
    <SectionWrapper>
      <div
        class="flex flex-col items-center justify-center gap-4 text-white text-center"
      >
        <h1 class="text-7xl">Wo Holz auf<br /> Kunst trifft</h1>
        <h4 class="text-3xl">
          Entdecken Sie die Schönheit maßgeschneiderter Tischlerei
        </h4>
      </div>
    </SectionWrapper>

    <SectionWrapper>
      <div class="bg-[#271d1d] text-[#f5d196] rounded-lg">
        <div class="grid grid-cols-1 sm:grid-cols-2">
          <h2 class="text-4xl p-4">Ein Erbe hochwertiger Tischlerei</h2>
          <p class="text-xl p-4">
            Mit jahrelanger Erfahrung und einer Leidenschaft für Tischlerei
            streben wir danach, außergewöhnliche Qualität und persönlichen
            Service zu bieten. Unser Engagement für Qualität, Liebe zum Detail
            und Kundenzufriedenheit hebt uns von anderen ab
          </p>
        </div>
        <div class="border-1 border-[#f5d196] mx-6 my-8"></div>
        <WorkDetails />
      </div>
    </SectionWrapper>

    <SectionWrapper>
      <div
        class="bg-[#271d1d] text-[#f5d196] text-center text-4xl py-2 px-4 rounded-lg"
      >
        Aktuelle Projekte
      </div>
    </SectionWrapper>

    <SectionWrapper>
      <Projects />
    </SectionWrapper>

    <Footer />
  </main>
</div>

<style>
  .main-bg {
    background-image: url("./assets/background.png");
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    background-attachment: fixed;
    position: relative;
    height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    overflow: hidden;
  }

  #main {
    background-color: transparent;
    width: 100%;
    height: 100%;
    scroll-behavior: smooth;
    overflow-y: auto;
    overflow-x: hidden;
  }
</style>
