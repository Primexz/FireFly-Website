<template>

  <vue-particles></vue-particles>

  <div class="bg-gray-900">

    <div class="d-flex justify-content-center text-white pt-24">

      <h1 style="font-weight: 900;" class="sm:text-5xl text-3xl text-center">

        <section class="hero container max-w-screen-lg mx-auto pb-10 flex justify-center w-5/12 sm:w-3/12 px-4 ">
          <img src="bot_logo.png" alt="FireFly-Logo"
               class="mx-auto shadow rounded-full max-w-full h-auto align-middle border-none"/>
        </section>

        <span><span
            style="color:#5663f7;">FireFly</span> | Incredible Music Experience</span>
      </h1>
    </div>
    <div class="d-flex justify-content-center subtext sm:text-3xl text-xl">
      <p style="font-style: italic;">The best Discord bot with the highest audio quality you've ever used!</p>

    </div>

    <div class="flex justify-center" style="margin-top: -19em; padding-bottom: 15em">
      <button style="z-index: 0;"
              onclick="window.location.href='https://discord.com/api/oauth2/authorize?client_id=925731507388174367&permissions=8&scope=bot%20applications.commands'"
              class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-3 px-4 mt-100 rounded-full ">
        Invite me
      </button>
    </div>


  </div>

  <svg class="bg-gray-800" style="fill: rgba(17, 24, 39, 1); transform: rotate(-180deg);"
       xmlns="http://www.w3.org/2000/svg" x="0px" y="0px"
       viewBox="0 0 1440 140">

    <path d="M685.6,52.8C418.7,2.9,170.2,23.9,0,44v96h1440V44C1252.7,66.2,1010,113.4,685.6,52.8z"
    ></path>
  </svg>


  <div class="bg-gray-800" id="features">

    <div class="d-flex justify-content-center text-white">
      <h1 style="font-weight: 900;">

        <span style="font-size: 40px;">Features</span>
      </h1>
    </div>

    <div class="container pt-5">
      <div class="row align-items-center">
        <div class="col-md-5 col-lg-6 order-md-1 order-0"><img
            class="w-100 flex items-center justify-center shadow rounded-2xl" src="images/help_cmd.png"
            alt=""/></div>
        <div class="col-md-7 col-lg-6 pe-lg-4 pe-xl-7">
          <div class="d-flex align-items-start"><img class="me-4"
                                                     src="https://cdn.discordapp.com/emojis/850924066517155871.png?v=1"
                                                     alt="" width="30"/>
            <div class="flex-1 text-white">
              <h5>All necessary commands for your server!</h5>
              <p class="text-muted mb-4">Are you tired of being bombarded by many commands all the time?<br>
                FireFly combines all important commands into a centrally categorized overview!</p>
            </div>
          </div>
        </div>
      </div>
    </div>


    <div class="container">
      <div class="row align-items-center mt-5">
        <div class="col-md-5 col-lg-6 order-md-0 order-1"><img class="w-100 shadow rounded-2xl"
                                                               src="images/music_filter.png"
                                                               alt=""/></div>
        <div class="col-md-7 col-lg-6 pe-lg-4 pe-xl-7">
          <div class="d-flex align-items-start"><img class="me-4"
                                                     src="https://cdn.discordapp.com/emojis/850924929444610048.png?v=1"
                                                     alt="" width="30"/>
            <div class="flex-1 text-white">
              <h5>The best music experience with our wide range of music filters!</h5>
              <p class="text-muted mb-4">We use FFmpeg to give you the best possible audio quality, without lags and
                delays.</p>
            </div>
          </div>
        </div>
      </div>
    </div>


    <div class="container">
      <div class="row align-items-center mt-5">
        <div class="col-md-5 col-lg-6 order-md-1 order-0"><img class="w-100 shadow rounded-2xl"
                                                               src="images/site_support.png"
                                                               alt=""/></div>
        <div class="col-md-7 col-lg-6 pe-lg-4 pe-xl-7">
          <div class="d-flex align-items-start"><img class="me-4"
                                                     src="https://cdn.discordapp.com/emojis/850831345051762719.png?v=1"
                                                     alt="" width="30"/>
            <div class="flex-1 text-white">
              <h5>Spotify, YouTube, Soundcloud ...</h5>
              <p class="text-muted mb-4">We support music streaming on all major music streaming sites to provide the
                best possible user experience.</p>
            </div>
          </div>
        </div>
      </div>
    </div>


    <div class="container">
      <div class="row align-items-center mt-5">
        <div class="col-md-5 col-lg-6 order-md-0 order-1"><img class="w-100 shadow rounded-2xl"
                                                               src="images/music_mng.png"
                                                               alt=""/></div>
        <div class="col-md-7 col-lg-6 pe-lg-4 pe-xl-7">
          <div class="d-flex align-items-start"><img class="me-4"
                                                     src="https://cdn.discordapp.com/emojis/853006694312574977.png?v=1"
                                                     alt="" width="30"/>
            <div class="flex-1 text-white">
              <h5>Modern Embeds with Button Interactions</h5>
              <p class="text-muted mb-4">FireFly uses all the new technologies of Discord. This includes <b>slash
                commands</b>, <b>button interactions</b> and much more.</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

</template>

<script>
export default {
  name: "Mainpage"
}
</script>

<style scoped>

#particles-js {
  position: absolute;
  background-size: cover;
  overflow-y: hidden;
  z-index: 0;
  width: 100%;
  height: 85vh;
}

.head {
  line-height: 1.3;
  text-align: center;
}

.subtext {
  padding-bottom: 330px;
  color: rgb(255, 255, 255, .55);
  line-height: 1.3;
  text-align: center;

}

.container {
  max-width: 1300px;
}

</style>