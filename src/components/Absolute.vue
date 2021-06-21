<template>
  <section class="container-fluid debugCont">
      <div class="jumbo-txt">
          <h1>Financial Risk</h1>
          <p>the right outcome depend on continuos rigor in governance, models, and processes across the finance function</p>
          <div>
              <div class="btn active">get in touch</div>
              <div class="btn">read more</div>
          </div>
      </div>
      <div class="carousel">
          <div class="empty"></div>
          <div class="full"></div>
          <div class="empty"></div>
      </div>
  </section>
</template>

<script>
export default {
    name: "Absolute"
}
</script>

<style lang="scss" scoped>
@import "../style/vars.scss";

.debugCont {
    text-align: center;
    color: #fff;
    height: calc(100% - 144px);
    position: relative;
    .jumbo-txt {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        h1 {
            font-size: 65px;
            font-weight: 800;
        }
        p {
            margin: 32px 0;
        }
        .btn {
            margin: 0 16px;
            padding: 8px 24px;
            border: 1px solid $primary-color;
            color: #fff;
            text-transform: uppercase;
            font-weight: 600;
        }
        .active {
            background-color: $primary-color;
            border: 0;
        }
        .btn:hover {
            background-color: $primary-color;
        }

    }
    .carousel {
        position: absolute;
        top: 50%;
        right: 0;
        transform: translate(0, -50%);
        
        .empty,
        .full {
            height: 20px;
            width: 10px;
            border: 1px solid $primary-color;
            border-radius: 50px;
            margin: 8px 0;
            cursor: pointer;
        }
        .full {
            background-color: $primary-color;
            border: 0;
        }
    }
}

</style>