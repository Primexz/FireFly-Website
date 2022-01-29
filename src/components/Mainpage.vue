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
            style="color:#5663f7;">FireFly</span> | Ultimate Music Experience</span>
      </h1>
    </div>
    <div class="d-flex justify-content-center subtext sm:text-3xl text-xl">
      <p style="font-style: italic;">The Best Music Bot with the Best, Highest Quality you ever
        used!</p>
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
        <div class="col-md-5 col-lg-6 order-md-1 order-0"><img class="w-100 shadow rounded-2xl" src="images/help_cmd.png"
                                                               alt=""/></div>
        <div class="col-md-7 col-lg-6 pe-lg-4 pe-xl-7">
          <div class="d-flex align-items-start"><img class="me-4"
                                                     src="https://cdn.discordapp.com/emojis/850924066517155871.png?v=1"
                                                     alt="" width="30"/>
            <div class="flex-1 text-white">
              <h5>All needed Commands for your Server</h5>
              <p class="text-muted mb-4">Are you sick of having a Music Bot with thousands Commands? Musicium has all
                Commands needed in just one Single Bot!
                <br> Tho they don't see like "much" you can use our Command structures to add one of the <b>2
                  Filters!</b></p>
            </div>
          </div>
        </div>
      </div>
    </div>


    <div class="container">
      <div class="row align-items-center mt-5">
        <div class="col-md-5 col-lg-6 order-md-0 order-1"><img class="w-100 shadow rounded-2xl" src="images/music_filter.png"
                                                               alt=""/></div>
        <div class="col-md-7 col-lg-6 pe-lg-4 pe-xl-7">
          <div class="d-flex align-items-start"><img class="me-4"
                                                     src="https://cdn.discordapp.com/emojis/850924929444610048.png?v=1"
                                                     alt="" width="30"/>
            <div class="flex-1 text-white">
              <h5>Ultimate Music Experiences means, 2Filters to adjust your Audio!</h5>
              <p class="text-muted mb-4">We are using FFMPEG, to give you the highest Audio Quality possible! As a
                matter of fact, we spawn them instantly and have no lag at all!</p>
            </div>
          </div>
        </div>
      </div>
    </div>


    <div class="container">
      <div class="row align-items-center mt-5">
        <div class="col-md-5 col-lg-6 order-md-1 order-0"><img class="w-100 shadow rounded-2xl" src="https://miro.medium.com/max/1000/1*IbcfLFZI_T0ajdrJVgNrVg.png"
                                                               alt=""/></div>
        <div class="col-md-7 col-lg-6 pe-lg-4 pe-xl-7">
          <div class="d-flex align-items-start"><img class="me-4"
                                                     src="https://cdn.discordapp.com/emojis/850831345051762719.png?v=1"
                                                     alt="" width="30"/>
            <div class="flex-1 text-white">
              <h5>Spotify, Soundcloud, Youtube, and 1100+ Other Links Supported!</h5>
              <p class="text-muted mb-4">We Support everything you listen to!
                INCLUDING PLAYLISTS AND <b>20 PREDEFINED, optimized, PLAYLISTS! (mix)</b></p>
            </div>
          </div>
        </div>
      </div>
    </div>


    <div class="container">
      <div class="row align-items-center mt-5">
        <div class="col-md-5 col-lg-6 order-md-0 order-1"><img class="w-100 shadow rounded-2xl" src="images/music_mng.png"
                                                               alt=""/></div>
        <div class="col-md-7 col-lg-6 pe-lg-4 pe-xl-7">
          <div class="d-flex align-items-start"><img class="me-4"
                                                     src="https://cdn.discordapp.com/emojis/853006694312574977.png?v=1"
                                                     alt="" width="30"/>
            <div class="flex-1 text-white">
              <h5>Clear Interface, with Logs and instant Buttons!</h5>
              <p class="text-muted mb-4">So that you can get all you want instantly from the Bot, and see everything
                what/who happened!</p>
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