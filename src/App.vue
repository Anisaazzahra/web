<template>
  <div>
    <section class="ft">
      <b-col class="dpn">
        <b-navbar-brand class="text-center mt-4"><h3>Profile Website</h3></b-navbar-brand>
        <div class="mt-4" style="float:right;">
          <b-button v-b-toggle.sidebar-right>
            
      <b-icon icon="three-dots-vertical" animation="cylon-vertical" font-scale="1"></b-icon>
          </b-button>
          <b-sidebar id="sidebar-right" title="Estetika" bg-variant="dark" text-variant="light" right shadow>
            <div class="px-3 py-2">
              <img src="./assets/Aristoteles.jpg" class="sdr" alt="Aristoteles">
              <p>{{side}}
              </p>
            </div>
          </b-sidebar>
        </div>

        <img class="mt-5 circle mx-auto d-block" alt="Profile Photo" src="./assets/pp.jpg"
          style="border-radius:50%; width:125px; height:125px;">
        <h1 class="text-center mt-4">Anisa Azzahra</h1>
        <p class="text-center mt-4">First Try To Create a Profile Website with VueJS</p>
      </b-col>

      <div class="mt-5 col-lg-12 mb-4 mt-4 px-4">
        <h1 class="text-left mt-4 mb-4">Intro</h1>
        <p class="text-left mt-4 mb-4">{{aboutText}}</p>
      </div>

      <div class="mt-5 col-lg-12 mb-4 mt-4 px-4">

        <h1 class="text-center mt-4 pb-4"><u>Education</u></h1>
        <b-card-group deck class="mt-4">
          <b-card header="SDN MELONG MANDIRI 1" header-bg-variant="dark" header-text-variant="white" align="center"
            style="border:transparent;">
            <img src="./assets/sd.png" style="height:35%;">
            <b-card-text class="mt-4"><b>Tahun 2008 - 2014</b></b-card-text>
          </b-card>

          <b-card header="SMP NEGERI 4 CIMAHI" header-bg-variant="dark" header-text-variant="white" align="center"
            style="border:transparent;">
            <img src="./assets/smp.png" style="height:35%;">
            <b-card-text class="mt-4"><b>Tahun 2014 - 2017</b></b-card-text>
          </b-card>

          <b-card header="SMK NEGERI 11 BANDUNG" header-bg-variant="dark" header-text-variant="white" align="center"
            style="border:transparent;">
            <img src="./assets/smk.png" style="height:35%;">
            <b-card-text class="mt-4"><b>Tahun 2017 - 2020</b></b-card-text>
          </b-card>
        </b-card-group>
      </div>
    
      
      <div class="mt-5 col-sm-14 mb-4 mt-4 px-4">

        <h1 class="text-center mt-4 pb-4"><u>Gallery</u></h1>
        <b-card-group deck class="mt-4">
          <b-card align="center" style="border:transparent;">
            <img class="col-12 col-md-6 col-lg-6" src="./assets/corbyn.jpg" alt="Corbyn Besson" style="width:200px;">
          </b-card>

          <b-card align="center" style="border:transparent;">
            <img class="col-12 col-md-6 col-lg-6" src="./assets/daniel.jpg" alt="Seavey Daniel" style="width:210px;">
          </b-card>

          <b-card align="center" style="border:transparent;" >
            <img class="col-12 col-md-6 col-lg-6" src="./assets/jack.jpg" alt="Jack Avery" style="width:200px;">
          </b-card><br>
          
        </b-card-group>
      </div>

      
      <div class="mt-5 col-sm-14 mb-4 mt-2 px-4">
        <b-card-group deck class="mt-4">

          <b-card align="center" style="border:transparent;">
            <img class="col-12 col-md-6 col-lg-6" src="./assets/seavey.png" alt="Seavey Daniel" style="width:200px;">
          </b-card>
          <b-card align="center" style="border:transparent;">
            <img class="col-12 col-md-6 col-lg-6" src="./assets/corbyn.jpg" alt="Corbyn Besson" style="width:200px;">
          </b-card>

          <b-card align="center" style="border:transparent;" >
            <img class="col-12 col-md-6 col-lg-6" src="./assets/daniel.jpg" alt="Jack Avery" style="width:210px;">
          </b-card><br>
          
        </b-card-group>
      </div>

      <div class="d-flex bg-dark text-light align-items-center px-3 py-2">
        <strong class="mx-auto" aria-colspan="12">&copy; {{ new Date().getFullYear() }} -  Anisa Azzahra </strong>
       </div>
    </section>

  </div>
</template>

<script>
  export default {

    data() {
      return {
        aboutText: "I enjoy building apps in my free time when I'm not doing much. I'm not very smart, just curious to see how things work. I'm also not that good of a writer as you can see. lol. Stay Healthy, Safe, And I hope you have a great day!",
        side: "Secara umum estetika dapat diartikan sebagai salah satu area dalam filsafat yang mencoba mengeksplorasi konsep keindahan/kecantikan yang berhubungan dengan atau terdapat dalam seni. Aristoteles mengatakan bahwa estetika merupakan fungsi atau manfaat dari seni dalam menciptkan pengalaman yang menyenangkan.",
        pht:{
          src :"./assets/sd.png" ,
        },
      }
    }
  }
</script>

<style>
  .dpn {
    padding-bottom: 100px;
    background-image: url('./assets/bk.jpg');
    background-position: center center;
    background-size: cover;
    color: white;
  }

  .pgr {
    float: right;
    border: 1px solid white;
    color: white;
  }

  .ft {
    line-height: 2;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  }
  .sdr{
    height: 50%;
    float: right;
  }
  .pht{
    width: 250px;
  }
  
</style>