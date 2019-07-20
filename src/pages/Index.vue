<template>
  <Layout>
    <div class="hero container-inner mx-auto flex flex-col sm:flex-row justify-between py-16">
      <div class="text-4xl font-bold w-full sm:w-3/5 text-center sm:text-left">
        <div class="leading-tight">Reuben Koppenheffer</div>
        <div class="text-purple-700 leading-tight">Web Developer</div>
      </div>
      <div class="mt-8 sm:mt-0">
        <g-image src="../../static/developer.svg" alt="hero" class="mx-auto sm:mx-0" />
      </div>
    </div>
    <!-- end hero -->

    <div class="container-inner mx-auto">
      <p
        class="text-lg sm:text-xl"
      >Hi! I'm Reuben, web developer extraordinaire. The time I'm not developing is spent creating photographs and relaxing with my family.</p>
      <div class="flex justify-between items-center py-6">
        <div class="w-full sm:w-1/2 px-8 py-8 sm:py-0">
          <g-image src="../../static/mind_map.svg" alt="browser" />
        </div>
        <div class="w-1/2 px-8 hidden sm:flex justify-end">
          <g-image src="../../static/code_review.svg" alt="mobile" />
        </div>
      </div>
    </div>

    <div class="overflow-x-hidden">
      <div
        class="projects container-inner mx-auto text-xl border-t border-gray-500 border-b py-16 mb-16 relative"
      >
        <h2 class="font-bold mb-6" id="projects">Here are some projects I've worked on:</h2>

        <div class="absolute right-0" style="top: 50px; transform: translate(100%) rotate(180deg)">
          <svg width="170px" height="170px">
            <use xlink:href="#dots-triangle" />
          </svg>
        </div>

        <ul class="text-lg sm:text-xl">
          <li class="checkmark mb-6">
            <div>Vue.js eBay Damage Tracking Web App</div>
            <div class="text-lg text-gray-600">
              This is a redesign of a Python 3 console app I created.
              It allows for entry of product and shipping losses for online sales and phsyical warehouse losses.
              It presents easy to view and modify data to help create loss reports. Uses Vue.js, Firebase, CSS, and Javascript.
              <a
                href="https://github.com/reuben-john/Simple-Damage-Tracking"
              >Github</a> --
              <a href="https://fir-damage-tracker.firebaseapp.com/">Live Demo</a>.
            </div>
          </li>
          <li class="checkmark mb-6">
            <div>Retro Portfolio</div>
            <div class="text-lg text-gray-600">
              Previous mockup of portfolio website with a retro feel. Built with HTML and CSS.
              <a
                href="https://github.com/reuben-john/html-css-templates/tree/master/retro-clone"
              >Github</a> and
              <a href="https://reuben-john.github.io/html-css-templates/retro-clone/">Live Demo</a>
            </div>
          </li>
          <li class="checkmark mb-6">
            <div>Bootstrap Portfolio</div>
            <div class="text-lg text-gray-600">
              This was my portfolio up until July 2019. Built using HTML, CSS, and Bootstrap.
              <a
                href="https://github.com/reuben-john/reuben-john.github.io"
              >Github</a> and
              <a href="https://reuben-john.netlify.com">Live Demo</a>
            </div>
          </li>
        </ul>
      </div>
      <!-- end projects -->
    </div>

    <div class="overflow-x-hidden border-gray-200 border-b">
      <div class="get-to-know-me container-inner mx-auto text-xl pb-16 relative">
        <h2 class="font-bold mb-6" id="about">Get to know me:</h2>

        <div class="absolute left-0" style="top: 50px; transform: translateX(-100%)">
          <svg width="170px" height="170px">
            <use xlink:href="#dots-triangle" />
          </svg>
        </div>

        <div class="flex flex-col sm:flex-row justify-between items-center mb-16">
          <div>
            <g-image
              src="../../static/reuben-john.jpg"
              alt="Photograph of Reuben"
              class="w-32 h-32 rounded-full mb-8 lg:mb-0"
            />
          </div>
          <div class="flex-1 text-lg sm:text-xl ml-6">
            I spent most of my working life managing a small business where I had to wear many hats to fit many different roles.
            The role that I found myself most in love with was Web Development.
            The first time I put together a website was a life altering experience.
            Since then, I have been growing and developing my skill set as a developer.
          </div>
        </div>
      </div>
      <!-- end get-to-know me -->
    </div>

    <div class="overflow-x-hidden">
      <div class="contact-me bg-background-secondary pt-16">
        <div class="container-inner mx-auto text-xl pb-4 relative">
          <h2 class="font-bold mb-6" id="contact">Contact me:</h2>

          <div class="absolute right-0 top-0" style="transform: translate(100%) rotate(180deg)">
            <svg width="170px" height="170px">
              <use xlink:href="#dots-triangle" />
            </svg>
          </div>

          <div class="text-lg sm:text-lg mb-16">
            <form
              name="contact"
              action="#"
              class="mb-12"
              method="POST"
              data-netlify="true"
              netlify-honeypot="bot-pot"
            >
              <input type="hidden" name="bot-pot" />
              <div class="flex flex-wrap mb-6 -mx-4">
                <div class="w-full md:w-1/2 mb-6 md:mb-0 px-4">
                  <label class="block mb-2 text-copy-primary" for="name">Name</label>

                  <input
                    type="text"
                    name="name"
                    id="name"
                    placeholder="John Smith"
                    class="block w-full bg-background-form border border-border-color-primary shadow rounded outline-none focus:border-purple-700 mb-2 p-4"
                    required
                  />
                </div>

                <div class="w-full px-4 md:w-1/2">
                  <label class="block text-copy-primary mb-2" for="email">Email Address</label>

                  <input
                    type="email"
                    name="email"
                    id="email"
                    placeholder="email@example.com"
                    class="block w-full bg-background-form border border-border-color-primary shadow rounded outline-none focus:border-purple-700 mb-2 p-4"
                    required
                  />
                </div>
              </div>

              <div class="w-full mb-12">
                <label class="block text-copy-primary mb-2" for="message">Message</label>

                <textarea
                  id="message"
                  rows="5"
                  name="message"
                  class="block w-full bg-background-form border border-border-color-primary shadow rounded outline-none appearance-none focus:border-purple-700 mb-2 px-4 py-4"
                  placeholder="Enter your message here."
                  required
                ></textarea>
              </div>

              <div class="flex justify-end w-full">
                <input
                  type="submit"
                  value="Submit"
                  class="block bg-purple-700 hover:bg-purple-800 text-white text-sm font-semibold tracking-wide uppercase shadow rounded cursor-pointer px-6 py-3"
                />
              </div>
            </form>
          </div>
        </div>
      </div>
      <!-- end contact-me -->
    </div>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: "Home"
  }
};
</script>

