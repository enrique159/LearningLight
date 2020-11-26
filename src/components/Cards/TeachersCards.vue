<template>
  <v-row>
    <v-col cols="12" class="columna" v-for="profe in profesores" :key="profe.nombre">
      <div class="tarjeta">
          <img
            :src="profe.foto"
            class="perfil"
            alt=""
          />
          <div class="datosProfesor">
            <h6>{{profe.nombre}}</h6>
            <span>{{profe.exp}} años de experiencia</span>
          </div>
          <div class="calificacion">
            <span>{{profe.calif}} </span>
          </div>
        </div>
    </v-col>
  </v-row>
</template>

<script>
export default {
  data() {
    return {
      profesores: [
        {
          nombre: "Edgar Aguilar",
          foto:
            "https://res.cloudinary.com/enrique159/image/upload/c_fill,h_258,w_258/v1606415306/Captura_de_Pantalla_2020-11-26_a_la_s_11.27.40_mkmzbk.png",
          exp: "5",
          calif: 4.8,
        },
        {
          nombre: "Alberto Matamoros",
          foto:
            "https://res.cloudinary.com/enrique159/image/upload/c_fill,h_1500,w_1500/v1606412501/MG_8139_ixockm.jpg",
          exp: "3",
          calif: 4.2,
        },
        {
          nombre: "Sarah Figueroa",
          foto:
            "https://res.cloudinary.com/enrique159/image/upload/c_fill,g_face:center,h_417,w_417,x_496,y_0/v1606412674/sonriente-jovencita-camiseta-disenada-buen-humor-pelo-largo-blanco_140725-14573_oy4ex7.jpg",
          exp: "7",
          calif: 5.2,
        },
        {
          nombre: "Patricia Armendariz",
          foto:
            "https://res.cloudinary.com/enrique159/image/upload/v1606413105/tlfhcpsxaowcsj8npnxr.jpg",
          exp: "2",
          calif: 4.5,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.columna{
  padding: 7px 12px;
}
.tarjeta {
  .perfil {
    height: 68px;
    border-radius: 34px;
  }
  .datosProfesor {
    padding: 14px 16px;
    display: inline-block;
    position: absolute;
    h6 {
      font-size: 14px;
      font-weight: 500;
      color: rgb(64, 42, 101);
    }
    span {
      font-size: 12px;
      color: #614e81;
    }
  }
  .calificacion{
    position: relative;
    float: right;
    padding: 18px 0px;
    span{
      color: #525ADF;
      font-size: 18px;
      font-weight: 500;
    }
  }
}
</style>