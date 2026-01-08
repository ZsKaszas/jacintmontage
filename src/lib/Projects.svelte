<script>
  import project1 from "../assets/project-1.jpg";
  import project2 from "../assets/project-2.jpg";
  import project3 from "../assets/project-3.jpg";
  import project4 from "../assets/project-4.jpg";
  import project5 from "../assets/project-5.jpg";
  import project6 from "../assets/project-6.jpg";
  import project7 from "../assets/project-7.jpg";
  import project8 from "../assets/project-8.jpg";
  import project9 from "../assets/project-9.jpg";
  import project10 from "../assets/project-10.jpg";
  import project11 from "../assets/project-11.jpg";
  import project12 from "../assets/project-12.jpg";
  import project13 from "../assets/project-13.jpg";
  import project14 from "../assets/project-14.jpg";
  import project15 from "../assets/project-15.jpg";
  import project16 from "../assets/project-16.jpg";
  import project17 from "../assets/project-17.jpg";
  import project18 from "../assets/project-18.jpg";
  import project19 from "../assets/project-19.jpg";
  import project20 from "../assets/project-20.jpg";
  import project21 from "../assets/project-21.jpg";
  import project22 from "../assets/project-22.jpg";
  import project23 from "../assets/project-23.jpg";
  import project24 from "../assets/project-24.jpg";
  import project25 from "../assets/project-25.jpg";
  import project26 from "../assets/project-26.jpg";
  import ImageWrapper from "./ImageWrapper.svelte";

  let images = [
    { src: project1, alt: "Project 1" },
    { src: project2, alt: "Project 2" },
    { src: project3, alt: "Project 3" },
    { src: project4, alt: "Project 4" },
    { src: project5, alt: "Project 5" },
    { src: project6, alt: "Project 6" },
    { src: project7, alt: "Project 7" },
    { src: project8, alt: "Project 8" },
    { src: project9, alt: "Project 9" },
    { src: project10, alt: "Project 10" },
    { src: project11, alt: "Project 11" },
    { src: project12, alt: "Project 12" },
    { src: project14, alt: "Project 14" },
    { src: project13, alt: "Project 13" },
    { src: project15, alt: "Project 15" },
    { src: project16, alt: "Project 16" },
    { src: project17, alt: "Project 17" },
    { src: project18, alt: "Project 18" },
    { src: project19, alt: "Project 19" },
    { src: project20, alt: "Project 20" },
    { src: project26, alt: "Project 26" },
    { src: project21, alt: "Project 21" },
    { src: project22, alt: "Project 22" },
    { src: project23, alt: "Project 23" },
    { src: project24, alt: "Project 24" },
    { src: project25, alt: "Project 25" }, 
  ];
</script>

<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
  {#each images as image}
    <ImageWrapper {image} />
  {/each}
</div>
