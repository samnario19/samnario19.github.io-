<script>
    import { Footer, FooterIcon }                                     from 'flowbite-svelte';
    import { FacebookSolid, GithubSolid, DiscordSolid, TwitterSolid } from 'flowbite-svelte-icons';
  </script>
  
    <Footer footerType="socialmedia" class="bg-transparent  relative z-20 pb-20">
        <hr class="my-6 border-gray-200 sm:mx-auto bg-transparent" />
        <div class="sm:flex sm:items-center sm:justify-between bg-transparent">
          <div class="flex mt-4 space-x-6 rtl:space-x-reverse sm:mt-0 justify-end w-full bg-transparent">
            <FooterIcon href="https://www.facebook.com/samnario19" class="bg-transparent">
              <FacebookSolid class="w-5 h-5 text-gray-500 dark:text-gray-500 hover:text-gray-900 dark:hover:text-white" />
            </FooterIcon>
            <FooterIcon href="/" class="bg-transparent">
              <DiscordSolid class="w-5 h-5 text-gray-500 dark:text-gray-500 hover:text-gray-900 dark:hover:text-white" />
            </FooterIcon>
            <FooterIcon href="/" class="bg-transparent">
              <TwitterSolid class="w-5 h-5 text-gray-500 dark:text-gray-500 hover:text-gray-900 dark:hover:text-white" />
            </FooterIcon>
            <FooterIcon href="https://github.com/samnario19" class="bg-transparent">
              <GithubSolid class="w-5 h-5 text-gray-500 dark:text-gray-500 hover:text-gray-900 dark:hover:text-white" />
            </FooterIcon>
          </div>
        </div>
      </Footer>
      
  