<!-- This is a NavBar with ButtonGroup -->
 <!-- I made this with the help of Chatgpt and flowbite -->

<script>
  import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
  import { ButtonGroup, Button }                          from 'flowbite-svelte';
  import { onMount }                                      from 'svelte';

  let navbarVisible = true; // State variable to track visibility of navbar

  // Function to set up the intersection observer
  function setupObserver() {
    const observer = new IntersectionObserver(
      (entries) => {
        entries.forEach((entry) => {
          navbarVisible = entry.isIntersecting; // Update the state based on intersection
        });
      },
      {
        root: null, // Use the viewport as the root
        threshold: 0, // Trigger when even a pixel is visible
      }
    );

    // Observe the navbar element
    const navbarElement = document.querySelector('#navbar');
    if (navbarElement) {
      observer.observe(navbarElement);
    }
  }

  // Run the observer setup on component mount
  onMount(() => {
    setupObserver();
  });
</script>

<style>
  .hidden {
    display: none;
  }
</style>

<!-- Navbar -->
<Navbar id="navbar" class="container mx-auto flex justify-between items-center p-4 bg-transparent">
  <NavBrand href="https://www.facebook.com/samnario19">
    <span class="text-2xl font-bold text-purple-500">Nandy Nario</span>
  </NavBrand>
  <NavHamburger />
  <NavUl>
    <NavLi class="text-2xl font-bold text-purple-200" href="/" active={true}>Home</NavLi>
    <NavLi class="text-2xl font-bold text-purple-200" href="/portfolio-page">Portfolio</NavLi>
    <NavLi class="text-2xl font-bold text-purple-200" href="/about-page">About</NavLi>
  </NavUl>
</Navbar>

<!-- Button Group at the Bottom -->
<div class="fixed bottom-0 inset-x-0 mx-auto mb-4 w-full flex justify-center z-10" class:hidden={navbarVisible}>
  <ButtonGroup class="*:!ring-primary-700">
    <Button color="dark" class="text-white" href="/">Home</Button>
    <Button color="dark" class="text-white" href="/portfolio-page">Portfolio</Button>
    <Button color="dark" class="text-white" href="/about-page">About</Button>
  </ButtonGroup>
</div>
