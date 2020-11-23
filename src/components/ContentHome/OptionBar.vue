<template>
  <v-container fluid>
    <v-row class="linea">
      <div v-for="clase in clases" :key="clase.clase">
        <v-btn
          v-if="clase.activo == false"
          class="boton botonNoSelected"
          depressed
        >
          <span>
            {{ clase.clase }}
          </span>
        </v-btn>
        <v-btn v-else class="boton botonSelected" depressed>
          <span>
            {{ clase.clase }}
          </span>
        </v-btn>
      </div>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      clases: [
        {
          clase: "Inglés",
          activo: false,
        },
        {
          clase: "Álgebra Lineal",
          activo: false,
        },
        {
          clase: "Bases de Tipografía",
          activo: false,
        },
        {
          clase: "Diseño UX/UI",
          activo: true,
        },
        {
          clase: "Taller de Diseño",
          activo: false,
        },
        {
          clase: "Scrum Management",
          activo: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.linea {
  padding: 16px 32px;

  .boton {
    margin: 12px 8px 12px;
    padding: 4px 10px;
    border-radius: 12px;
    span {
      text-transform: none;
      letter-spacing: 0;
    }
  }

  .botonNoSelected {
    background-color: #eff0ff !important;
    span {
      color: rgb(64, 42, 101);
    }
  }

  .botonSelected {
    background-color: rgb(80, 87, 222) !important;
    span {
      color: white;
    }
  }
}
</style>