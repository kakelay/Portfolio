 
<template>
  <div class="bg-white">
    <Header> </Header>
  </div>

  <div class="bg-white">
    <div
      class="mx-auto grid max-w-2xl grid-cols-1 items-center gap-x-8 gap-y-16 px-4 py-24 sm:px-6 sm:py-32 lg:max-w-7xl lg:grid-cols-2 lg:px-8"
    >
      <div>
        <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl  ">
          This is my project
        </h2>
        <p class="mt-4 text-gray-500">
          The walnut wood card tray is precision milled to perfectly fit a stack
          of Focus cards. The powder coated steel divider separates active cards
          from new ones, or can be used to archive important task lists.
        </p>

        <dl
          class="mt-16 grid grid-cols-1 gap-x-6 gap-y-10 sm:grid-cols-2 sm:gap-y-16 lg:gap-x-8"
        >
          <div
            v-for="feature in features"
            :key="feature.name"
            class="border-t border-gray-200 pt-4"
          >
            <dt class="font-medium text-gray-900">{{ feature.name }}</dt>
            <dd class="mt-2 text-sm text-gray-500">
              {{ feature.description }}
            </dd>
          </div>
        </dl>
      </div>

      <div class="grid grid-cols-2 grid-rows-2 gap-4 sm:gap-6 lg:gap-8">
        <img
          src="https://avatars.githubusercontent.com/u/110383694?v=4"
          alt="Walnut card tray with white powder coated steel divider and 3 punchout holes."
          class="rounded-lg bg-gray-100"
        />
        <img
          src="https://avatars.githubusercontent.com/u/110383694?v=4"
          alt="Top down view of walnut card tray with embedded magnets and card groove."
          class="rounded-lg bg-gray-100"
        />
        <img
         src="https://avatars.githubusercontent.com/u/110383694?v=4"
          alt="Side of walnut card tray with card groove and recessed card area."
          class="rounded-lg bg-gray-100"
        />
        <img
          src="https://avatars.githubusercontent.com/u/110383694?v=4"
          alt="Walnut card tray filled with cards and card angled in dedicated groove."
          class="rounded-lg bg-gray-400"
        />
      </div>
    </div>
  </div>

  <div class="bg-gray-100">
    <Footer></Footer>
  </div>
</template>





<script >
import Header from "~/components/Header.vue";
import Footer from "~/components/Footer.vue";

export default {
  components: {
    Header,
    Footer,
  },
};
</script>
