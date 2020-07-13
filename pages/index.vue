<template>
  <div class="text-gray-600 font-body">
    <div>
      <nav>
        <div>
          <h1 class="font-bold uppercase">
            <a href="/">Food Ninja</a>
          </h1>
        </div>
        <ul>
          <li>
            <a href="#">
              <span>Home</span>
            </a>
          </li>
          <li>
            <a href="#">
              <span>About</span>
            </a>
          </li>
          <li>
            <a href="#">
              <span>Contact</span>
            </a>
          </li>
        </ul>
      </nav>
    </div>
  
    <main class="px-16 py-16">
      <div class="flex justify-end">
        <a href="#" class="text-orange-600">Log in</a>
        <a href="#" class="text-orange-600">Sign up</a>
      </div>

      <header>
        <h2 class="text-gray-700 text-6xl font-semibold">Recipes</h2>
        <h3 class="text-2xl font-semibold">For Ninjas</h3>
      </header>

      <div>
        <h4 class="font-bold">Latest Recipes</h4>
  
        <div>
          <!-- cards go here -->
          <div> 
            <img src="~/assets/stew.jpg" alt="stew">
            <div>
              <span>5 Bean Chili Stew</span>
              <span>Recipe by Mario</span>
            </div>
          </div>
        </div>

        <h4 class="font-bold">Most Popular</h4>

        <div>
          <!-- cards go here -->
        </div>
      </div>

      <div class="flex justify-center">
        <div>Load more</div>
      </div>    
    </main>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>

</style>