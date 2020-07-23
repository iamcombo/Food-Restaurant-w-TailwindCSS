<template>
  <div class="text-gray-600 font-body">
    <div class="grid md:grid-cols-3">
      <div class="md:col-span-1 md:flex md:justify-end">
        <nav class="text-right">
          <div class="flex justify-between items-center">
            <h1 class="font-bold uppercase p-4 border-b border-gray-100">
              <a href="/" class="hover:text-gray-700">Food PISET</a>
            </h1>
            <div class="px-4 cursor-pointer md:hidden" @click="handleNav">
              <svg class="w-6" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h6a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z" clip-rule="evenodd"></path></svg>
            </div>
          </div>
          <ul class="text-sm mt-6 md:block" v-if="nav">
            <li class="text-gray-700 font-bold py-2">
              <a href="#" class="flex justify-end px-4 border-r-4 border-orange-500">
                <span>Home</span>
                <svg class="w-5 ml-2" fill="currentColor" viewBox="0 0 20 20"><path d="M10.707 2.293a1 1 0 00-1.414 0l-7 7a1 1 0 001.414 1.414L4 10.414V17a1 1 0 001 1h2a1 1 0 001-1v-2a1 1 0 011-1h2a1 1 0 011 1v2a1 1 0 001 1h2a1 1 0 001-1v-6.586l.293.293a1 1 0 001.414-1.414l-7-7z"></path></svg>
              </a>
            </li>
            <li class="py-2">
              <a href="#" class="flex justify-end px-4 border-r-4 border-white">
                <span>About</span>
                <svg class="w-5 ml-2" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M18 10a8 8 0 11-16 0 8 8 0 0116 0zm-8-3a1 1 0 00-.867.5 1 1 0 11-1.731-1A3 3 0 0113 8a3.001 3.001 0 01-2 2.83V11a1 1 0 11-2 0v-1a1 1 0 011-1 1 1 0 100-2zm0 8a1 1 0 100-2 1 1 0 000 2z" clip-rule="evenodd"></path></svg>
              </a>
            </li>
            <li class="py-2">
              <a href="#" class="flex justify-end px-4 border-r-4 border-white">
                <span>Contact</span>
                <svg class="w-5 ml-2" fill="currentColor" viewBox="0 0 20 20"><path d="M2.003 5.884L10 9.882l7.997-3.998A2 2 0 0016 4H4a2 2 0 00-1.997 1.884z"></path><path d="M18 8.118l-8 4-8-4V14a2 2 0 002 2h12a2 2 0 002-2V8.118z"></path></svg>
              </a>
            </li>
          </ul>
        </nav>
      </div>
    
      <main class="px-16 py-16 bg-gray-100 md:col-span-2">
        <div class="flex justify-center md:justify-end">
          <a href="#" class="text-orange-600 btn border-orange-600 md:border-2 hover:bg-orange-600 hover:text-white transition ease-in-out duration-500">Log in</a>
          <a href="#" class="text-orange-600 ml-2 btn border-orange-600 md:border-2 hover:bg-orange-600 hover:text-white transition ease-in-out duration-500">Sign up</a>
        </div>

        <header>
          <h2 class="text-gray-700 text-6xl font-semibold">Recipes</h2>
          <h3 class="text-2xl font-semibold">For Ninjas</h3>
        </header>

        <div>
          <h4 class="font-bold">Latest Recipes</h4>
          <hr class="mx-4">
          <div class="mt-8 grid lg:grid-cols-3 gap-10">
            <!-- cards go here -->
            <div class="card hover:shadow-lg"> 
              <img src="~/assets/stew.jpg" alt="stew" class="w-full h-32 sm:h-48 object-cover">
              <div class="m-4">
                <span class="font-bold">5 Bean Chili Stew</span>
                <span class="block">Recipe by Mario</span>
              </div>
              <div class="badge">
                <svg class="w-5 inline-block" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm1-12a1 1 0 10-2 0v4a1 1 0 00.293.707l2.828 2.829a1 1 0 101.415-1.415L11 9.586V6z" clip-rule="evenodd"></path></svg>
                <span>25 mins</span>
              </div>
            </div>
            <div class="card hover:shadow-lg"> 
              <img src="~/assets/curry.jpg" alt="stew" class="w-full h-32 sm:h-48 object-cover">
              <div class="m-4">
                <span class="font-bold">5 Bean Chili Stew</span>
                <span class="block">Recipe by Mario</span>
              </div>
              <div class="badge">
                <svg class="w-5 inline-block" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm1-12a1 1 0 10-2 0v4a1 1 0 00.293.707l2.828 2.829a1 1 0 101.415-1.415L11 9.586V6z" clip-rule="evenodd"></path></svg>
                <span>25 mins</span>
              </div>
            </div>
            <div class="card hover:shadow-lg"> 
              <img src="~/assets/noodles.jpg" alt="stew" class="w-full h-32 sm:h-48 object-cover">
              <div class="m-4">
                <span class="font-bold">5 Bean Chili Stew</span>
                <span class="block">Recipe by Mario</span>
              </div>
              <div class="badge">
                <svg class="w-5 inline-block" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm1-12a1 1 0 10-2 0v4a1 1 0 00.293.707l2.828 2.829a1 1 0 101.415-1.415L11 9.586V6z" clip-rule="evenodd"></path></svg>
                <span>25 mins</span>
              </div>
            </div>
          </div>

          <h4 class="font-bold mt-8">Most Popular</h4>
          <hr class="mx-4">
          <div>
            <!-- cards go here -->
          </div>
        </div>

        <div class="flex justify-center mt-8">
          <div class="btn bg-blue-400 text-white hover:shadow-inner transform hover:scale-125 hover:bg-opacity-50 transition ease-out duration-300">Load more</div>
        </div>    
      </main>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      nav: false
    }
  },
  methods: {
    handleNav() {
      this.nav = !this.nav
    }
  }
}
</script>