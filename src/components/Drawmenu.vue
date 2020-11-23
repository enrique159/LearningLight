<template>
  <div class="drawmenu">
    <v-container>
      <div class="espacio"></div>
      <v-col v-for="opcion in menu" :key="opcion.accion" class="opcion">
        <v-btn class="opcionbtn" depressed color="#FFFFFF">
          <v-row align="center">
            <v-icon medium :color="opcion.color">
              {{ opcion.icono }}
            </v-icon>
            <span :style="{ color: opcion.color }">{{ opcion.accion }}</span>
          </v-row>
        </v-btn>
      </v-col>
      <div id="espacio2"></div>
    </v-container>
    <div class="linea"></div>
    <MisTareas/>
  </div>
</template>

<script>
import MisTareas from './DrawMenu/MisTareas'

export default {
  data() {
    return {
      menu: [
        {
          accion: "Inicio",
          icono: "mdi-home",
          color: "#525ADF",
        },
        {
          accion: "Cursos",
          icono: "mdi-school",
          color: "#7B63A4",
        },
        {
          accion: "Entrenamiento",
          icono: "mdi-brain",
          color: "#7B63A4",
        },
        {
          accion: "Estadísticas",
          icono: "mdi-chart-arc",
          color: "#7B63A4",
        },
        {
          accion: "Ajustes",
          icono: "mdi-cog-outline",
          color: "#7B63A4",
        },
      ],
    };
  },
  components:{
    MisTareas,
  }
};
</script>

<style lang="scss">
.drawmenu {
  border-right: 2px solid rgb(239, 240, 255);
  width: 256px;
  height: 100vh;
  max-height: 100vh;
  position: fixed;
  float:left;

  .espacio {
    margin-top: 82px;
  }

  #espacio2 {
    margin-top: 24px;
  }

  .linea {
    border-bottom: 2px solid rgb(239, 240, 255);
  }

  .opcion {
    padding: 8px 4px;
    .opcionbtn {
      width: 100%;
      text-transform: none;
      letter-spacing: normal;
      span {
        color: #7b63a4;
        padding-top: 3px;
        padding-left: 8px;
      }
    }
  }
}
</style>