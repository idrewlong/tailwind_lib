<div class="flex flex-col items-center justify-center min-h-screen">
        <h1 class="text-4xl font-bold">Welcome to ID-DEV Tailwind Library</h1>
        <h2 class="text-xl font-thin italic mt-2">Under Construction</h2>
        <section class="grid grid-cols-1 md:grid-cols-3 md:space-x-4">
                <div class=" flex flex-col space-y-6 py-4">
                        <div class="flex flex-col justify-center items-center"><h1>Sections</h1></div>
                        <a href="/" class="button_home">Nav</a>
                        <a href="/hero" class="button_home">Hero</a>
                        <a href="/" class="button_home">About</a>
                        <a href="/" class="button_home">Features</a>
                        <a href="/cta" class="button_home">CTA</a>
                        <a href="/" class="button_home">Footers</a>
                </div>
                <div class=" flex flex-col space-y-6 py-4">
                        <div class="flex flex-col justify-center items-center"><h1>Components</h1></div>
                        <a href="/hero" class="button_home">Buttons</a>
                        <a href="/" class="button_home">Cards</a>
                </div>
                <div class=" flex flex-col space-y-6 py-4">
                        <div class="flex flex-col justify-center items-center"><h1>Templates</h1></div>
                        <a href="/" class="button_home">Agency</a>
                        <a href="/" class="button_home">Portfolio</a>
                        <a href="/" class="button_home">Video Studio</a>
                        <a href="/" class="button_home">Audio Engineer</a>
                </div>
        </section>
        
</div>

<style>
        .button_home {
	@apply px-6 py-3 rounded-lg shadow-xl bg-orange-400 hover:opacity-80 duration-200 transition-opacity text-center;
}

</style>