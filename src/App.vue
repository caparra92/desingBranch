<template>
  <div id="app">
    <div class="w-4/5 mx-auto my-0 p-0">
      <MainHeader title="social media post" subtitle="Business Events" />
      <div class="flex">
        <div class="w-1/2 p-5 m-5 mb-0 mr-0">
          <Card class="shadow-2xl">
            <template v-slot:cardHeader>
              <div class="w-full font-semibold">
                <MainHeader title="business" subtitle="events" color="yellow-500" size="5" pl="8" />
              </div>
            </template>
            <template v-slot:cardContent>
              <div class="w-full flex m-5 mt-0 pt-0">
                <div class="w-1/3 ml-5 mt-10 pt-10">
                  <h1 class="font-bold text-4xl text-left">2020</h1>
                  <TextContent />
                </div>
                <div class="w-2/3 pl-8 m-10 p-5 ml-2">
                  <img
                    :src="require('./assets/img/cupgirl.png')"
                    alt="cupgirl"
                    class="border-8 border-yellow-500"
                  />
                </div>
              </div>
            </template>
          </Card>
        </div>
        <div class="w-1/2 p-5 m-5 mb-0 ml-0">
          <div class="flex">
            <div class="w-1/2 pr-2 mr-2">
              <!--  segundo card -->
              <Card class="shadow-2xl flex" gradient="wb">
                <template v-slot:cardHeader>
                  <div class="w-full mt-0 pt-0">
                    <div class="w-full font-semibold text-blue-600">
                      <MainHeader
                        title="business"
                        subtitle="events"
                        color="yellow-500"
                        titleSize="1"
                        size="2"
                        pl="3"
                      />
                    </div>
                    <div class="w-full py-2 pl-2 ml-5 pr-5">
                      <img
                        :src="require('./assets/img/writinggirl.png')"
                        alt="cupgirl"
                        class="border-4 border-yellow-500"
                      />
                    </div>
                  </div>
                </template>
                <template v-slot:cardContent>
                  <div class="w-full ml-5 py-5 pt-2">
                    <div class="w-full ml-2 pt-5 pr-5">
                      <img
                        :src="require('./assets/img/writinggirl2.png')"
                        alt="cupgirl"
                        class="border-4 border-yellow-500"
                      />
                    </div>
                    <div class="w-full py-2 pl-2 leading-tight">
                      <TextContent />
                    </div>
                  </div>
                </template>
              </Card>
            </div>
            <!-- terceiro card -->
            <div class="w-1/2 pl-1">
              <Card class="shadow-2xl" gradient="shape">
                <template v-slot:cardHeader>
                  <div class="w-full text-yellow-500">
                    <Frame/>
                  </div>
                </template>
                <template v-slot:cardContent>
                  <div class="w-full flex p-5 mt-20 bg-blue-800">
                    <div class="w-full font-semibold">
                      <MainHeader
                        title="business"
                        subtitle="events"
                        color="yellow-500"
                        titleSize="1"
                        size="2"
                        pl="3"
                      />
                    </div>
                    <div class="w-full leading-tight">
                      <TextContent />
                    </div>
                  </div>
                </template>
              </Card>
            </div>
          </div>
          <!-- quarto card -->
          <div class="flex">
            <div class="w-1/2 pr-5 mr-5">
              <Card class="shadow-2xl" gradient="shape2">
                <template v-slot:cardHeader>
                  <div class="w-full text-yellow-500">
                    <Cone/>
                  </div>
                </template>
                <template v-slot:cardContent>
                  <div class="w-full flex m-5 mt-0 pt-0">
                    <div class="w-1/3">
                      <TextContent />
                    </div>
                  </div>
                </template>
              </Card>
            </div>
            <!-- quinto card -->
            <div class="w-1/2">
              <Card class="shadow-2xl">
                <template v-slot:cardHeader>
                  <div class="w-full font-semibold">
                    <MainHeader title="business" subtitle="events" color="yellow-400" />
                  </div>
                </template>
                <template v-slot:cardContent>
                  <div class="w-full flex m-5 mt-0 pt-0">
                    <div class="w-1/3">
                      <TextContent />
                    </div>
                    <div class="w-2/3">
                      <img :src="require('./assets/img/cupgirl.png')" alt="cupgirl" />
                    </div>
                  </div>
                </template>
              </Card>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Card from "@/components/Card.vue";
import MainHeader from "@/components/MainHeader.vue";
import TextContent from "@/components/TextContent.vue";
import Frame from "@/components/Frame.vue";
import Cone from "@/components/Cone.vue";

export default {
  name: "App",
  components: {
    Card,
    MainHeader,
    TextContent,
    Frame,
    Cone
  }
};
</script>

<style>
#app {
  font-family: "Roboto", sans-serif;
  text-align: center;
  color: #fff;
  background: linear-gradient(135deg, #004a89 50%, #fdbe42 50%);
  background-size: cover;
  height: 100vh;
  width: 100vw;
  /* primarycolor #004a89 azul*/
  /* secondary  #fdbe42 amarelo*/
}
</style>
