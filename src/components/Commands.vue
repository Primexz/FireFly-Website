<template>

  <svg class="bg-gray-900" style="fill: rgba(31, 41, 55, 1);
  ; transform: rotate(-180deg);"
       xmlns="http://www.w3.org/2000/svg" x="0px" y="0px"
       viewBox="0 0 1440 140">

    <path d="M685.6,52.8C418.7,2.9,170.2,23.9,0,44v96h1440V44C1252.7,66.2,1010,113.4,685.6,52.8z"
    ></path>
  </svg>

  <div class="bg-gray-900" id="commands">

    <div class="w-6/12 mx-auto">
      <div class="shadow-sm">

        <div class="d-flex justify-content-center text-white">
          <h1 style="font-weight: 900;">

            <span style="font-size: 40px;">Commands</span>
          </h1>
        </div>

        <div class="pt-10">


          <div v-for="(categorie, index) in commandCategories" :key="index">

            <div class="text-white">
              <h1 style="font-weight: 900;">
                <span style="font-size: 20px;">{{ categorie }}</span>
              </h1>
            </div>


            <!-- looped commands -->
            <div v-for='command in commands[index]' :key="command"
                 class="transition hover:bg-gray-800 rounded-2xl mt-2">
              <!-- header -->
              <div
                  class="accordion-header cursor-pointer transition flex space-x-5 px-5 items-center h-16 text-gray-400">
                <i class="fas fa-plus"></i>
                <h3> {{ command.name }} </h3>
              </div>
              <!-- Content -->
              <div class="accordion-content sm:px-5 pt-0  overflow-hidden max-h-0 bg-gray-800 text-white rounded-2xl">
                <p class="leading-6 font-light pl-9 text-justify sm:text-base text-sm">
                  {{ command.description }}
                </p>
                <a class="px-6 py-2 my-5 ml-9">
                </a>
              </div>
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
      commandCategories: [
        "Music Commands",
        "Activity Commands",
        "Fun Commands",
        "Other Commands"
      ],

      commands: [
        [
          {
            name: "play",
            description: "Add song to music queue"
          },
          {
            name: "manager",
            description: "Manage your current queue"
          },
          {
            name: "filter",
            description: "Manage all music filters/effects"
          },
          {
            name: "nowplaying",
            description: "Get information about the song that is currently playing."
          },
          {
            name: "volume",
            description: "Set the volume of the current song in percent"
          },
          {
            name: "queue",
            description: "Get an overview of the songs that are currently added to the queue."
          },
        ],

        [
          {
            name: "betrayal",
            description: 'Create a "betrayal" game!'
          },
          {
            name: "checkers",
            description: 'Create a "checkers" game!'
          },
          {
            name: "chess",
            description: 'Create a "Chess In The Park" game!'
          },
          {
            name: "doodle-crew",
            description: "Create a doodle-crew game! (Game like Skribbl)"
          },
          {
            name: "fishington",
            description: 'Create a "fishington" game!'
          },
          {
            name: "letterleague",
            description: 'Create a "letterleague" game!'
          },
          {
            name: "poker",
            description: 'Create a "poker" game!'
          },
          {
            name: "spellcast",
            description: 'Create a "spellcast" game!'
          },
          {
            name: "watch-together",
            description: 'Create a "watch-together" game!'
          },
          {
            name: "wordsnacks",
            description: 'Create a "wordsnacks" game!'
          },
        ],
        [
          {
            name: "ttt",
            description: "Play TicTacToe with a teammate"
          }
        ],
        [
          {
            name: "help",
            description: 'Get information about all the commands of FireFly.'
          },
          {
            name: "avatar",
            description: 'Get avatar image & url from an user'
          },
          {
            name: "stats",
            description: 'Get statistics about FireFly'
          },
          {
            name: "shards",
            description: "Get an overview of the current shards from FireFly."
          },
        ]
      ],
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