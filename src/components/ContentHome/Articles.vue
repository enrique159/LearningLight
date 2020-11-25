<template>
  <v-container fluid>
    <v-row class="contenedor">
      <v-col cols="8" class="columna">
        <v-row class="titulo">
          <h4>Artículos <span>162</span></h4>
        </v-row>
        <v-row class="cards articles">
          <v-col>
            <ArticlesCards />
          </v-col>
        </v-row>
      </v-col>
      <v-col cols="4" class="columna">
        <v-row class="titulo">
          <h4>Chats de Temas <span>12</span></h4>
        </v-row>
        <v-row class="cards">
          <v-col>
            <ThemesCards />
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import ArticlesCards from "../Cards/ArticlesCards";
import ThemesCards from "../Cards/ThemesCards";

export default {
  data() {
    return {};
  },
  components: {
    ArticlesCards,
    ThemesCards,
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
}
</style>