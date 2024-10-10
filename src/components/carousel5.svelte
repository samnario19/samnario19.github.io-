<script>
    import { Carousel } from 'flowbite-svelte';
  
    const images = [
      {
        alt: 'My First Image',
        src: 'images/cater1.jpg',
        title: 'Image 1 Description'
      },
      {
        alt: 'My Second Image',
        src: 'images/cater2.jpg',
        title: 'Image 2 Description'
      },
      {
        alt: 'My Third Image',
        src: 'images/cater3.jpg',
        title: 'Image 3 Description'
      },
      {
        alt: 'My Fourth Image',
        src: 'images/kape1.jpg',
        title: 'Image 4 Description'
      },
      {
        alt: 'My Fifth Image',
        src: 'images/kape3.jpg',
        title: 'Image 5 Description'
      },
      {
        alt: 'My Sixth Image',
        src: 'images/kape4.jpg',
        title: 'Image 6 Description'
      },
      {
        alt: 'My Seventh Image',
        src: 'images/light1.jpg',
        title: 'Image 7 Description'
      },
      {
        alt: 'My Eighth Image',
        src: 'images/lights2.png',
        title: 'Image 8 Description'
      },
      // Add more images as needed
    ];
  </script>
  
  <!-- Carousel container -->
  <div class="flex items-center justify-center w-full h-screen">
    <div class="max-w-4xl w-full space-y-4">
    <h1 class="text-5xl font-bold mb-4 text-purple-400">My Work Photos</h1>
      <Carousel {images} imgClass="object-contain h-full w-fit rounded-sm" let:Indicators let:Controls class="rounded-md ring-4 ring-purple-500 border-4 border-white dark:border-gray-800 min-h-[320px] bg-transparent">
        <Indicators class="border border-white rounded-md p-2" />
        <Controls class="items-center text-red-400 dark:text-purple-400 pt-4" />
      </Carousel>
    </div>
  </div>  