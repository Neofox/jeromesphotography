<script>
  import main_picture from '$lib/images/600.png';
  import portrait_picture from '$lib/images/600.png';
  import landscape_picture from '$lib/images/600.png';
  import street_picture from '$lib/images/600.png';
  import form_picture from '$lib/images/600.png';
</script>

<svelte:head>
  <title>Home</title>
  <meta name="description" content="Jerome Schaeffer Photography" />
</svelte:head>

<section>
  <div class="grid grid-cols-2 h-screen">
    <div class="hidden md:block col-span-1">
      <img class="h-screen w-full object-cover" src={main_picture} alt="Main Self Portrait" />
    </div>
    <div class="ml-8 md:ml-12 lg:ml-20 col-span-2 md:col-span-1">
      <div class="absolute right-0 mt-4 mr-4 z-10">
        <a class="hover:text-yellow-500 hover:underline cursor-pointer" href="#">FR</a>
        /
        <a class="text-yellow-700 hover:text-yellow-500 hover:underline cursor-pointer" href="#">EN</a>
        /
        <a class="hover:text-yellow-500 hover:underline cursor-pointer" href="#">KO</a>
      </div>

      <div class="relative left-0 mt-4">
        <a class="text-xs hover:text-yellow-500 hover:underline" href="http://github.com/Neofox">
          Want to see my Web Development projects?
        </a>
      </div>
      <div class="font-bold text-5xl lg:text-6xl my-12 mr-8 uppercase">
        <h1 class="leading-snug">Hello, I'm Jerome.</h1>
        <h1 class="">Photographer,</h1>
        <h1 class="">Videographer,</h1>
        <h1 class="">Traveler.</h1>
      </div>
      <p class="mr-14 my-16">
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aliquid ad in consectetur nesciunt suscipit laudantium
        molestias illo sit facere optio. Recusandae at omnis numquam aperiam laudantium rerum debitis, dignissimos
        architecto.
      </p>

      <a
        href="#gallery"
        class="block border-l-4 p-4 uppercase font-semibold border-orange-300 hover:bg-orange-100 w-fit	transition-colors"
      >
        Gallery
      </a>
      <a
        href="#contact"
        class="block px-4 py-2 border-l-4 mt-8 uppercase font-semibold border-gray-500 hover:bg-gray-300 w-fit transition-colors"
      >
        Contact Us
      </a>
    </div>
  </div>

  <div id="gallery" class="my-28 mx-20">
    <div class="text-center">
      <h2 class="text-5xl uppercase font-bold">My Work</h2>
      <p class="mx-80 my-14">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Aspernatur explicabo laboriosam asperiores
        exercitationem illo dolor nisi natus obcaecati. Dignissimos deserunt facere sed nam praesentium nostrum a velit
        enim aspernatur quo.
      </p>
    </div>

    <div class="grid grid-cols-3 gap-5">
      <div class="col-span-1">
        <div class="relative transition-all duration-300 cursor-pointer filter grayscale hover:grayscale-0">
          <a href="/">
            <img class="rouded-lg" src={portrait_picture} alt="Portrait" />
          </a>
          <h3 class="absolute px-4 text-lg text-white bottom-6">Portrait Photography</h3>
        </div>
      </div>
      <div class="col-span-1">
        <div class="relative transition-all duration-300 cursor-pointer filter grayscale hover:grayscale-0">
          <a href="/">
            <img class="rouded-lg" src={street_picture} alt="Street" />
          </a>
          <h3 class="absolute px-4 text-lg text-white bottom-6">Street Photography</h3>
        </div>
      </div>
      <div class="col-span-1">
        <div class="relative transition-all duration-300 cursor-pointer filter grayscale hover:grayscale-0">
          <a href="/">
            <img class="rouded-lg" src={landscape_picture} alt="Landscape" />
          </a>
          <h3 class="absolute px-4 text-lg text-white bottom-6">Landscape Photography</h3>
        </div>
      </div>
    </div>
  </div>

  <div id="contact" class="mt-28 mb-10 mx-20 text-center">
    <h2 class="text-4xl uppercase font-bold">Want to work with me?</h2>
    <p class="mx-80 my-14">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam, doloremque labore. Consequatur praesentium officia
      eaque placeat voluptate iusto, beatae sed.
    </p>
    <div class="grid grid-cols-3 gap-5">
      <div class="col-span-1">
        <img class="w-full object-cover" src={form_picture} alt="Send form" />
      </div>
      <div class="col-span-2 mx-16">
        <form>
          <div class="mb-6">
            <label for="email" class="block mb-2 text-sm font-medium text-left">Email</label>
            <input
              id="email"
              class="bg-gray-100 border border-gray-300 text-sm rounded-lg focus:ring-yellow-500 focus:border-yellow-500 block w-full p-2.5"
              type="email"
              placeholder="contact@gmail.com"
              required
            />
          </div>
          <div>
            <label for="message" class="block mb-2 text-sm font-medium text-left">Ask me anything</label>
            <textarea
              id="message"
              class="bg-gray-100 border border-gray-300 text-sm rounded-lg focus:ring-yellow-500 focus:border-yellow-500 block w-full p-2.5"
              rows="4"
              placeholder="..."
              required
            />
          </div>
          <div class="mt-6 text-left">
            <button
              class="text-white bg-yellow-400 hover:bg-yellow-600 focus:ring-4 focus:outline-none focus:ring-yellow-100 font-medium rounded-lg text-sm w-full sm:w-3/6 px-5 py-2.5 text-center"
              >Send</button
            >
          </div>
        </form>
      </div>
    </div>
  </div>
</section>
