<template>
  <div class="container cards-cont">
      <div class="cards p-4">
        <img class="mb-3" src="../assets/images/logo.svg" alt="logo">
        <div v-for="data,index in dataOne" :key="index">
            <p> {{data}} </p>
        </div>
        <div class="btn">get in touch</div>
      </div>
      <div class="cards mx-3 p-5 bg-gray">
          <h4>About</h4>
          <ul>
              <li v-for="data, index in dataTwo" :key="index">
                  <i class="fas fa-chevron-right"></i>
                    <a href="#">{{data}}</a>
              </li>
          </ul>
      </div>
      <div class="cards me-3 p-5 bg-gray">
        <h4>Services</h4>
            <ul>
                <li v-for="data, index in dataThree" :key="index">
                    <i class="fas fa-chevron-right"></i>
                    <a href="#">{{data}}</a>
                </li>
            </ul>
      </div>
      <div class="cards p-5 bg-gray">
          <h4>Support</h4>
            <ul>
                <li v-for="data, index in dataFour" :key="index">
                    <i class="fas fa-chevron-right"></i>
                    <a href="#">{{data}}</a>
                </li>
            </ul>
      </div>
  </div>
</template>

<script>
export default {
    name: "BottomCards",
    props: ["dataOne", "dataTwo", "dataThree", "dataFour"]
}
</script>

<style lang="scss" scoped>
@import "../style/vars.scss";

.cards-cont {
    height: 100%;
    display: flex;
    align-items: center;

    //stile di tutte le cards
    .bg-gray {
        background-color: rgba($color: #ccc, $alpha: 0.1);
    }
    .cards {
        width: calc(100% / 4);
        border-radius: 10px;
        height: 320px;
        color: #ccc;
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
        } //end stile della prima card
        h4 {
            margin-bottom: 16px;
            color: #fff;
        }
        ul {
            list-style: none;
            padding-left: 0;
            li {
                margin: 8px 0;                
                font-size: 16px;
                svg {
                    margin-right: 8px;
                }
                a {
                    color: #ccc;
                    text-decoration: none;
                    text-transform: capitalize;
                }
                a:hover {
                    color: #fff;
                }
    
            }
        }
    }

}

</style>