<script>


        import { onMount, onDestroy } from 'svelte';
            
              let slides = [
                { text: "Andrew Long", duration: 3000 },
                { text: "a React Developer", duration: 3000 },    
                { text: "a Svelte Developer ", duration: 3000 },  
                { text: "a Golang Developer", duration: 3000 },
                { text: "a Python Developer", duration: 3000 }
              ];
            
              let currentIndex = 0;
              let intervalId;
              const intervalDuration = 2000; // Default interval duration
            
              function replaceWord() {
                currentIndex = (currentIndex + 1) % slides.length;
              }
            
              onMount(() => {
                // Start the interval immediately upon mounting
                intervalId = setInterval(replaceWord, intervalDuration);
              });
            
              onDestroy(() => {
                clearInterval(intervalId);
              });
        </script>
        
        <header class="shadow-lg bg-gray-200 min-h-[30rem] rounded-3xl mb-8 flex justify-center items-center relative p-3 overflow-hidden max-w-7xl mx-auto">
                <img class="absolute left-0 top-0 min-h-full min-w-full" src="/bg_3.webp" alt="">
          
            <div class="container relative mx-auto lg:px-32">
              <div class="gap-12 flex flex-col md:flex-row items-center"> 
                <div class="p-4 text-center md:text-left md:mt-0 md:w-1/2 flex flex-col items-center md:items-start justify-center"> 
                
                  <h1 class="text-4xl md:text-6xl  font-bold tracking-tight mb-12">Hello, I am  <br /><span class="text-orange-400">{slides[currentIndex].text}</span></h1>
                
                  <div class="flex flex-col md:flex-row space-y-4 justify-center md:space-y-0 space-x-2"> 
                    <a class="flex bg-gradient-to-br from-yel_orange to-giants_orange md:px-4 py-2  text-white font-medium text-sm leading-snug uppercase rounded hover:opacity-80 hover:shadow-sm transition duration-300 justify-center text-center" data-mdb-ripple="true" data-mdb-ripple-color="light" href="https://www.linkedin.com/in/idrewlong" role="button">LinkedIn</a>
                    <a class="flex bg-transparent text-orange-400 font-medium text-sm leading-snug uppercase rounded px-4 py-2  hover:opacity-80 hover:shadow-sm transition duration-300 justify-center text-center" data-mdb-ripple="true" data-mdb-ripple-color="light" href="/resume" role="button">Resume</a>
                  </div>
                </div>
        
                <div class="mb-12 md:w-1/2 md:mb-0">
                  <img
                    src="drew2.webp"
                    class="w-full rounded-lg shadow-lg"
                    alt="Andrew Long"
                  />
                </div>
              </div>
            </div>
        </header>