<script>
  import Navbar             from '../../components/navbar.svelte';
  import Footer             from '../../components/footer.svelte'; 
  import Carousel5          from '../../components/carousel5.svelte';
</script>

<main>
  <Navbar />
  <section id="about" class="py-16 bg-transparent">
    <div class="container mx-auto px-4">
      <h1 class="text-4xl font-bold text-purple-500 mb-4">About Me</h1>
      <h2 class="text-2xl font-bold text-purple-400 mb-4">  Hey Hello! It's me again, Nandy Nario a passionate third-year Computer Science student at Gordon College 
        and I aspire to become a front-end developer in the future.</h2>
      <div class="flex flex-col md:flex-row items-center">
        <!-- About Me Content -->
        <div class="md:w-2/3 mb-8 md:mb-0">
          <p class="text-lg text-purple-300 mb-4 ">
            I'm currently working as a freelancer in non-IT fields, but I aspire to become a front-end developer in the future.
            such as Bartender, Waiter, Caterer and Lights and Sounds helper
          </p>     
           <p class="text-lg text-purple-300 mb-4 ">
            I also enjoy activities like buying and selling items, particularly bike parts. It’s a great way for me to earn money, 
            and I’m proud to have been able to help my family a little and buy the things I want throughout my college years through these endeavors.
          </p>
        </div>

        <!-- Profile Picture -->
        <div class="md:w-1/3 flex justify-center">
          <img src="images/profileko.png" alt="Profile pic" class="object-cover max-h-[60vh] rounded-lg shadow-lg" />
        </div>
      </div>
    </div>    
  </section>

  <section id="journey" class="py-16 bg-transparent">
    <div class="container mx-auto px-4">
      
      <h3 class="text-2xl text-purple-200 font-bold mb-4">My Journey as a Student Developer</h3>
      <p class="mb-4 ">
        As a third-year Computer Science student at Gordon College, my journey in the field of technology has been both challenging and rewarding. Over the past few years, I've immersed myself in various aspects of computer science, from core programming concepts to more specialized areas like web development and machine learning.
      </p>
      <p class="mb-4">
        My coursework has provided a solid foundation in algorithms, data structures, and software engineering principles. I’ve had the opportunity to work on diverse projects, which has allowed me to apply theoretical knowledge to practical problems. One of the highlights of my academic experience has been developing a blog application with Angular and PHP, which taught me a lot about full-stack development and user authentication.
      </p>
      <p class="mb-4">
        Outside the classroom, I’ve been actively involved in freelance work and personal projects. These experiences have not only honed my skills in front-end development but also improved my problem-solving abilities and time management. I’m particularly proud of the progress I’ve made in creating responsive, user-friendly interfaces and learning new technologies like Svelte.
      </p>
      <p class="mb-4">
        Looking ahead, I am excited to continue my journey toward becoming a front-end developer. I am eager to tackle new challenges, collaborate on innovative projects, and further develop my skills in creating dynamic and engaging web experiences.
      </p>
    </div>
  </section>

  <section class="py-16">
    <div class="text-center">
      <Carousel5 />
    </div>
  </section>
  
  

  <Footer />
</main>

<style>
  main {
    margin-top: 2rem;
  }
</style>
