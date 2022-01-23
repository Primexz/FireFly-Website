<template>
  <div class="bg-gray-900">

    <hr style="width: 75%;background-color: #FFFFFF!important;color: #FFFFFF!important;border: 5px solid #FFFFFF!important;border-radius:25px;margin-left: 12%;">

    <div class="w-6/12 mx-auto">
      <div class="p-10 shadow-sm">

        <div class="d-flex justify-content-center text-white">
          <h1 style="font-weight: 900;">

            <span style="font-size: 40px;">Commands</span>
          </h1>
        </div>

        <div class="pt-10">

          <!-- looped commands -->
          <div v-for="command in commands.music" :key="command" class="transition hover:bg-gray-800 rounded-2xl">
            <!-- header -->
            <div class="accordion-header cursor-pointer transition flex space-x-5 px-5 items-center h-16 text-gray-400">
              <i class="fas fa-plus"></i>
              <h3> {{ command.name }} </h3>
            </div>
            <!-- Content -->
            <div class="accordion-content px-5 pt-0 overflow-hidden max-h-0 bg-gray-800 text-white rounded-2xl">
              <p class="leading-6 font-light pl-9 text-justify">
                {{ command.description }}
              </p>
              <button class="rounded-full bg-indigo-600 text-white font-medium font-lg px-6 py-2 my-5 ml-9">Learn more
              </button>
            </div>
          </div>
        </div>

      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Commands",

  data: () => {
    return {
      commands: {
        music: [
          {
            name: "play",
            description: "Play an song"
          }
        ]
      }
    }
  },
  mounted() {
    const accordionHeader = document.querySelectorAll(".accordion-header");
    accordionHeader.forEach((header) => {
      header.addEventListener("click", function () {
        const accordionContent = header.parentElement.querySelector(".accordion-content");
        let accordionMaxHeight = accordionContent.style.maxHeight;

        if (accordionMaxHeight == "0px" || accordionMaxHeight.length == 0) {
          accordionContent.style.maxHeight = `${accordionContent.scrollHeight + 32}px`;
          header.querySelector(".fas").classList.remove("fa-plus");
          header.querySelector(".fas").classList.add("fa-minus");
          header.parentElement.classList.add("bg-gray-800");
        } else {
          accordionContent.style.maxHeight = `0px`;
          header.querySelector(".fas").classList.add("fa-plus");
          header.querySelector(".fas").classList.remove("fa-minus");
          header.parentElement.classList.remove("bg-gray-800");
        }
      });
    });
  }
}
</script>

<style scoped>
.accordion-content {
  transition: max-height 0.3s ease-out, padding 0.3s ease;
}
</style>