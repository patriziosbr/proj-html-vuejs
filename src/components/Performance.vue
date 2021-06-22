<template>
  <section class="container-fluid bg-white">
        <div class="mainHeading text-center mx-auto container">
            <h5 class="text-uppercase my-4" >introduction video</h5>
            <h1 class="my-4">Advisory <span>Performance</span></h1>
            <p class="my-5">Financial executievs need to review thei strategies, operating models and capabilities so that their arear can generate sound information for better decision making.</p>
            <div class="vid-cont my-5">
                <img src="../assets/images/video-1.jpg" alt="">
                <div class="layerAbs" ></div>
                <i class="fas fa-play green"></i>
                <i class="fas fa-play white"></i>
            </div>
      </div>
  </section>
</template>

<script>
export default {
    name: "Performance"
}
</script>

<style lang="scss" scoped>
@import "../style/vars.scss";

    .bg-white{
        background-color: #fff;
        .mainHeading {
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
                span {
                    padding: 4px 10px;
                    border-radius: 5px;
                    display: inline-block;
                    color: $primary-color;
                    background-color: rgba($color: $primary-color, $alpha: 0.3);
                }
            }
            p {
                font-size: 19px;
                line-height: 150%;
                color: #7D878E;
            }
        .vid-cont {
            position: relative;
            img {
                width: 100%;
            }
            .layerAbs {
                height: 100%;
                width: 100%;
                background-color: rgba($color: $primary-color, $alpha: 0.2);
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%, -50%);
            }
            .green {
                color: rgba($color: $primary-color, $alpha: 0.8);
                font-size: 64px;
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%, -50%);
            }
            .white {
                color: rgba($color: #fff, $alpha: 0.6);
                font-size: 64px;
                position: absolute;
                top: 52%;
                left: 50%;
                transform: translate(-50%, -50%);
            }
          }
        }
    }

</style>