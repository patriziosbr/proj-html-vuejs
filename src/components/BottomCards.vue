<template>
  <div class="container cards-cont">
      <div class="cards p-4">
        <img class="mb-3" src="../assets/images/logo.svg" alt="logo">
        <div v-for="data,index in dataOne" :key="index">
            <p> {{data}} </p>
        </div>
        <div class="btn">get in touch</div>
      </div>
      <div class="cards mx-3 p-4">
          <h4>About</h4>
      </div>
      <div class="cards me-3 p-4"></div>
      <div class="cards p-4"></div>
  </div>
</template>

<script>
export default {
    name: "BottomCards",
    props: ["dataOne"]
}
</script>

<style lang="scss" scoped>
@import "../style/vars.scss";

.cards-cont {
    height: 100%;
    display: flex;
    align-items: center;
    border: 1px solid #fff;
    //stile di tutte le cards
    .cards {
        width: calc(100% / 4);
        border: 1px solid red;
        height: 320px;
        color: #fff;
        font-size: 13px;
        img {
            height: 50px;
        }
        div:nth-child(3) p:before {
            font-family: "Font Awesome 5 Free";
            font-weight: 900;
            content: "\f879";
            margin-right: 8px;
        }
        div:nth-child(4) p:before {
            font-family: "Font Awesome 5 Free";
            font-weight: 900;
            content: "\f0e0";
            margin-right: 8px;
        }
        div:nth-child(5) p:before {
            font-family: "Font Awesome 5 Free";
            font-weight: 900;
            content: "\f3c5";
            margin-right: 8px;
        }
         .btn {
            padding: 8px 24px;
            border: 1px solid $primary-color;
            color: #fff;
            text-transform: uppercase;
            font-weight: 600;
        }
        .btn:hover {
            background-color: $primary-color;
        }
    } //end stile della prima card

}

</style>