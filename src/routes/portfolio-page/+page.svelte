<script>
  import    Navbar             from '../../components/navbar.svelte';
  import    Footer             from '../../components/footer.svelte';
  import    Carousel1          from '../../components/carousel1.svelte';
  import    Carousel2          from '../../components/carousel2.svelte';
  import    Carousel3          from '../../components/carousel3.svelte';
  import    Carousel4          from '../../components/carousel4.svelte'; 
  import { Progressbar }       from 'flowbite-svelte';
</script>

<main>
<Navbar />

<section class="py-16">
  <div class="text-center">
    <h1 class="text-5xl font-bold mb-4 text-purple-600">Welcome to My Portfolio</h1>
    <p class="text-xl text-purple-300">Here you will find information my projects.</p>
  </div>
</section>

<section class="py-16">
  <div class="text-center">
  <h2 class="text-5xl font-bold mb-4 text-purple-400">Bank Management system</h2>
  <p class="text-2xl text-purple-300">(PHP)</p>
  <Carousel1 />
  <div class="mb-1 text-base font-medium text-purple-300 dark:text-purple-400">100% COMPLETE</div>
  <div class="max-w-4xl mx-auto">
    <Progressbar progress="100" color="purple" />
  </div>
 </div>
</section>

<section class="py-16">
  <div class="text-center">
  <h3 class="text-5xl font-bold mb-4 text-purple-400">Weather Application</h3>
  <p class="text-2xl text-purple-300">(Angular)</p>
  <Carousel2 />
   <div class="mb-1 text-base font-medium text-purple-300 dark:text-purple-400">Progress 50%</div>
    <div class="max-w-4xl mx-auto">
      <Progressbar progress="50" color="purple" />
    </div>
   </div>
</section>

<section class="py-16">
  <div class="text-center">
  <h4 class="text-5xl font-bold mb-4 text-purple-400">Simple Blog Application</h4>
  <p class="text-2xl text-purple-300">(Angular)</p>
  <Carousel3 />
  <div class="mb-1 text-base font-medium text-purple-700 dark:text-purple-400">Progress 0%</div>
  <div class="max-w-4xl mx-auto">
    <Progressbar progress="0" color="purple" />
  </div>
 </div>
</section>

<section class="py-16">
  <div class="text-center">
  <h4 class="text-5xl font-bold mb-4 text-purple-400">Image Gallery</h4>
  <p class="text-2xl text-purple-300">(Angular)</p>
  <Carousel4 />
  <div class="mb-1 text-base font-medium text-purple-700 dark:text-purple-400">Progress 0%</div>
  <div class="max-w-4xl mx-auto">
    <Progressbar progress="0" color="purple" />
  </div>
 </div>
</section>




<Footer />
</main>

<style>
main {
  margin: 0;
  padding: 0;
}
</style>
