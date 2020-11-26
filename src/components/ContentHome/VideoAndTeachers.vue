<template>
  <v-container fluid>
    <v-row class="contenedor">
      <v-col cols="8" class="columna">
        <v-row class="titulo">
          <h4>Videos de lecciones <span>72</span></h4>
        </v-row>
        <v-row class="cards articles">
          <v-col>
            <VideoCards />
          </v-col>
        </v-row>
      </v-col>
      <v-col cols="4" class="columna">
        <v-btn class="opcionbtn" depressed color="#FFFFFF">
          <v-row align="center">
            <span id="tituloProf">Top Profesores</span>
            <v-icon id="ArrowRight" medium color="#525ADF">
              mdi-arrow-right
            </v-icon>
          </v-row>
        </v-btn>
        <v-row class="cards">
          <v-col>
            <TeachersCards />
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import VideoCards from "../Cards/VideoCards";
import TeachersCards from "../Cards/TeachersCards";

export default {
  data() {
    return {};
  },
  components: {
    VideoCards,
    TeachersCards,
  },
};
</script>

<style lang="scss" scoped>
.contenedor {
  padding: 0px 28px;
  max-width: 1280px;

  .columna {
    padding: 0px 12px;
  }
  .cards {
    padding-right: 24px;
  }
  .articles {
    max-width: 720px;
  }
  .titulo {
    padding: 0px 12px;
    h4 {
      padding-left: 2px;
      font-weight: 400;
      font-size: 18px;
      color: rgb(64, 42, 101);
      span {
        padding-left: 12px;
        font-size: 18px;
        font-weight: 600;
        color: rgb(80, 87, 222);
      }
    }
  }

  .opcionbtn {
    width: 100%;
    #tituloProf {
      text-transform: none;
      letter-spacing: normal;
      font-weight: 400;
      font-size: 18px;
      color: rgb(64, 42, 101);
      padding-top: 3px;
      padding-left: 8px;
    }
    #ArrowRight {
      position: absolute;
      right: 0px;
    }
  }
}
</style>