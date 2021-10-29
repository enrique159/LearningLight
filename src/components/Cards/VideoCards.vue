zerodown2d<template>
  <v-row>
    <v-col cols="7">
      <div
        class="tarjeta"
        style="
          background-image: url('https://res.cloudinary.com/zerodown2d/image/upload/v1606332898/bgp-01_jecn0t.png');
        "
      >
        <h2>We create effective<br />text for landing</h2>
        <div class="tiempo">
          <span class="minutos">10:08</span>
        </div>
        <div class="profesor">
          <img
            src="https://pbs.twimg.com/profile_images/974736784906248192/gPZwCbdS.jpg"
            class="perfil"
            alt=""
          />
          <div class="datosProfesor">
            <h6>Cristian Bane</h6>
            <span>CEO of TuBankflip</span>
          </div>
        </div>
      </div>
    </v-col>
    <v-col cols="5">
      <v-col class="columnas" cols="12">
        <div
          id="tarjeta1"
          class="tarjeta"
          style="
            background-image: url('https://res.cloudinary.com/zerodown2d/image/upload/v1606332898/bgp-02_gdtufg.png');
          "
        >
          <h3>Aprende a diseñar <br />tu Business Card</h3>
          <div class="profesor">
            <img
              src="https://lulusingles.com/uploads/2/5/k/w/tj195pt4jvxjgck4qce6_p.jpg"
              class="perfil"
              alt=""
            />
            <div class="datosProfesor">
              <h6>Daniel Alfonso</h6>
              <span>Senior Design</span>
            </div>
          </div>
        </div>
      </v-col>
      <v-col class="columnas" cols="12">
        <div
          id="tarjeta2"
          class="tarjeta"
          style="
            background-image: url('https://res.cloudinary.com/zerodown2d/image/upload/v1606332898/bgp-03_hvduii.png');
          "
        >
          <h3>Animaciones en<br />After Effects</h3>
          <div class="profesor">
            <img
              src="https://pixinvent.com/demo/vuexy-vuejs-admin-dashboard-template/demo-3/img/user-13.005c80e1.jpg"
              class="perfil"
              alt=""
            />
            <div class="datosProfesor">
              <h6>Ana McFlyy</h6>
              <span>Graphic Designer</span>
            </div>
          </div>
        </div>
      </v-col>
    </v-col>
  </v-row>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
#tarjeta1 {
  height: 152px;
  padding: 18px;
  background-position: bottom right;
}

#tarjeta2 {
  height: 152px;
  padding: 18px;
}

.columnas {
  padding: 0px 0px 24px;
}

.tarjeta {
  border-radius: 12px;
  background-position: top right;
  background-size: cover;
  position: relative;
  padding: 21px;
  height: 328px;

  h2 {
    font-weight: 500;
    font-size: 21px;
    color: rgb(255, 255, 255);
    margin-bottom: 21px;
  }
  
  h3{
    font-weight: 500;
    font-size: 16px;
    color: rgb(255, 255, 255);
    margin-bottom: 21px;
  }

  .tiempo {
    position: absolute;
    right: 20px;
    bottom: 21px;
    padding: 4px 4px 6px 6px;
    background-color: rgb(64, 42, 101);
    border-radius: 8px;
    color: #e4e5f5;
    width: fit-content;
    .minutos {
      font-size: 14px;
      font-weight: 600;
      padding: 0px 4px;
    }
  }

  .profesor {
    position: absolute;
    bottom: 16px;
    .perfil {
      height: 48px;
      border-radius: 12px;
    }
    .datosProfesor {
      padding: 0px 8px;
      float: right;
      padding-top: 6px;
      h6 {
        font-size: 14px;
        font-weight: 500;
        color: rgb(255, 255, 255);
      }
      span {
        font-size: 12px;
        color: #d6d6d6;
      }
    }
  }

  .ilustracion {
    position: absolute;
    top: 48px;
    right: 20px;
    img {
      height: 128px;
    }
  }
  .ilustracionSmall {
    position: absolute;
    top: 78px;
    right: 20px;
    img {
      height: 72px;
    }
  }
}
</style>