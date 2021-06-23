<template>
  <section class="container-fluid bg-green">
      <div class="container mainHeading">
          <h5 class="text-uppercase me-4">our editoria content</h5>
            <h3 class="my-1">Latest <span>News</span></h3>
            <div class="paragraph-cont">
                <p class="my-2">Every week we publish content about what is the business world</p>
                <div class="btn">see all</div>
            </div>
            <div class="container-cards">

                
                <div class="card bg-one">
                    <div class="layer d-flex align-content-between flex-wrap">
                        <div class="posted d-flex align-items-center justify-content-between hide">
                            <div class="d-flex align-items-center ">
                                <i class="far fa-user "></i>
                                <p class="m-0 ms-2  ">Andrea Miller</p>
                            </div>
                            <div class="d-flex align-items-center ms-5 ">
                                <i class="far fa-user "></i>
                                <p class="m-0 ms-2 ">Andrea Miller</p>
                            </div>
                        </div>
                        <div class="text-center">
                            <h4 class="my-4">Increasing creativity is possibile for everyone</h4>
                            <p class="hide">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, est.</p>
                        </div>
                    </div>
                </div>
                <div class="card bg-two">
                    <div class="layer d-flex align-content-between flex-wrap">
                        <div class="posted d-flex align-items-center justify-content-between hide">
                            <div class="d-flex align-items-center ">
                                <i class="far fa-user "></i>
                                <p class="m-0 ms-2  ">Andrea Miller</p>
                            </div>
                            <div class="d-flex align-items-center ms-5 ">
                                <i class="far fa-user "></i>
                                <p class="m-0 ms-2 ">Andrea Miller</p>
                            </div>
                        </div>
                        <div class="text-center">
                            <h4 class="my-4">Increasing creativity is possibile for everyone</h4>
                            <p class="hide">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, est.</p>
                        </div>
                    </div>
                </div>
                <div class="card bg-three">
                    <div class="layer d-flex align-content-between flex-wrap">
                        <div class="posted d-flex align-items-center justify-content-between hide">
                            <div class="d-flex align-items-center ">
                                <i class="far fa-user "></i>
                                <p class="m-0 ms-2  ">Andrea Miller</p>
                            </div>
                            <div class="d-flex align-items-center ms-5 ">
                                <i class="far fa-user "></i>
                                <p class="m-0 ms-2 ">Andrea Miller</p>
                            </div>
                        </div>
                        <div class="text-center">
                            <h4 class="my-4">Increasing creativity is possibile for everyone</h4>
                            <p class="hide">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, est.</p>
                        </div>
                    </div>
                </div>
            </div>
      </div>

  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import "../style/vars.scss";
.bg-green {
    background-color: $bg-green-lgt;
    padding: 64px;
    h5 {
        font-size: 18px;
        color: $primary-color;
        font-weight: 700;
    }
    h3 {
        font-size: 48px;
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
    .paragraph-cont {
        display: flex;
        align-items: center;
        justify-content: space-between;
        p {
            width: 80%;
            font-size: 16px;
            line-height: 150%;
            color: $bg-dark-gray ;
        }
        .btn {
            padding: 4px 24px;
            border: 1px solid $primary-color;
            color: #fff;
            text-transform: uppercase;
            font-weight: 600;
            background-color: $primary-color;
        }
        
    }
    .bg-one {
        background-image: url(../assets/images/news-1.jpg);
        background-size: cover;
        background-position: center;
        
    }
    .bg-two {
        background-image: url(../assets/images/news-2.jpg);
        background-size: cover;
        background-position: center;
    }
    .bg-three {
        background-image: url(../assets/images/news-3.jpg);
        background-size: cover;
        background-position: center;
    }
     .container-cards {
  
        // height: 400px;
        position: relative;
        margin: 32px 0;
        display: flex;
        justify-content: space-between;

        .card {
            width: calc(100% / 3 - 32px);
            height: 300px;
            .layer {
                padding: 40px;
                position: absolute;
                top: 0;
                left: 0;
                height: 100%;
                width: 100%;
                background-color: rgba($color: #000000, $alpha: 0.6);
                svg {
                    color: #fff;
                }
            }
        h4 {
            color: #fff;
            // position: absolute;
            // bottom: 0px;
            // left: 0;
            // transform: translate(0, -50%);
        }
        p {
            color: #fff;
            font-size: 18px;
        }
        .hide {
            visibility: hidden;
        }
        .layer:hover .hide {
            visibility: visible;
        }
      
        }
    }
}

</style>