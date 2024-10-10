  <script>
    import Button      from '../components/showcontact.svelte';
    import Navbar      from '../components/navbar.svelte';
    import Profile     from '../components/profile.svelte';
    import Footer      from '../components/footer.svelte';
  </script>

  <main>
    <Navbar />
    <Profile/>
    <section id="home" class="py-16">
      <div class="text-center">
        <h1 class="text-5xl font-bold text-purple-200 mb-4">Hi, I'm <span class="text-purple-500">Nandy Nario</span></h1>
        <h2 class="text-2xl font-bold text-purple-200 mb-4">Currently, I Am a Third Year College Student At Gordon College</h2>
        <p class="text-xl text-gray-200 mt-4"> </p>
      </div>
    </section>
    
    <section id="last" class="py-16">
      <div class="text-center">
        <h5 class="text-3xl font-bold text-purple-200 mb-4">And This Is My <span class="text-purple-500">Simple Portfolio</span> Made with Svelte</h5>
      </div>
    </section>
    
    <section id="scroll-info" class="py-16">
      <div class="text-center">
        <h6 class="text-3xl font-bold text-purple-200 mb-4">Explore My Work, Learn About My Journey</h6>
        <h7 class="text-xl font-bold text-purple-200 mb-2">(Feel Free To Reach Out If You'd Like To Connect Or Collaborate)</h7>
        <Button />
        </div> 

    <Footer/>
  </main>
  <style>
    main {
      margin-top: 2rem;
    }
  </style>