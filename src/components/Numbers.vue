<template>
  <section class="container-fluid bg-car">
      <div class="container text-center mx-auto heading-cars">
          <h5 class="text-uppercase my-4" >what are we doing</h5>
           <h1 class="my-4"><span>Results</span> in Numbers</h1>
           <div class="container-num d-flex">
               <div class="item-num" v-for="elem, index in numberitems" :key="index">
                   <h3>{{ elem.numInfo }}</h3>
                   <h4>{{ elem.txtInfo }}</h4>
               </div>
           </div>
      </div>
  </section>
</template>

<script>
export default {
    name: "Numbers",
    data() {
        return {
            numberitems : [
                {
                    numInfo: 128,
                    txtInfo: "certification"
                },
                {
                    numInfo: 230,
                    txtInfo: "Employees"
                },
                {
                    numInfo: 517,
                    txtInfo: "customers"
                },
                {
                    numInfo: 94,
                    txtInfo: "country served"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/vars.scss";

    .bg-car::before {
        content: "";
        position: absolute;
        top: 0; left: 0;
        width: 100%; height: 100%;
        background-image: url(../assets/images/cars.jpg);
        background-position: center;
        background-size: cover;
        filter: grayscale(100%) brightness(30%);
    }

    .bg-car {
        // height: 600px;
        position: relative;
        .heading-cars {
            position: relative;
            padding: 64px;
            h5 {
                font-size: 18px;
                color: $primary-color;
                font-weight: 700;
            }
            h1 {
                font-size: 56px;
                font-weight: 800;
                letter-spacing: 1px;
                color: #fff;
                span {
                    padding: 4px 10px;
                    border-radius: 5px;
                    display: inline-block;
                    background-color: rgba($color: $primary-color, $alpha: 0.3);
                }
            }
            .container-num {
                height: 300px;
                width: 100%;
                .item-num {
                    height: 100%;
                    width: calc(100% / 4);
                    display: flex;
                    justify-content: center;
                    flex-direction: column;
                    h3 {
                        color: $primary-color;
                        font-weight: 700;
                    }
                    h4 {
                        color: #fff;
                        text-transform: capitalize;
                    }

                }
            }
        }
    }

</style>