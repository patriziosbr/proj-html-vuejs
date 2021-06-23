<template>
  <section class="container-fluid bg-dark">

    <div class="container d-flex align-items-center justify-content-center">
      <div class=" mainHeading">
        <h5 class="text-uppercase mb-4">newsletter</h5>
        <h3 class="mb-4"><span>Know</span> Frist</h3>
        <p class="my-2">Follow closely and recive content about our company and the news of the current market.</p>
      </div>

      <div class="mainForm">
        <form action="post" class="d-flex flex-column">
          <input class="mb-4" type="text" name="name" id="name" placeholder="Name">
          <input class="mb-4" type="text" name="email" id="email" placeholder="Email">
          <div class="btn">subscribe</div>
        </form>
      </div>


    </div>

  </section>
</template>

<script>
export default {
  name: "Lead"

}
</script>

<style lang="scss" scoped>
@import "../style/vars.scss";
.bg-dark {
   background-color: $bg-dark-gray;

    padding: 64px;
.mainHeading {
  width: 45%;
  padding: 32px;
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
  p {
    color: #ccc;
  }
}
  .mainForm {
    width: 30%;
    input {
      padding: 12px 12px;
      background-color: $bg-form;
      box-shadow: none;
      border: none;
      border-radius: 5px;
    }
      .btn {
        width: 40%;
          padding: 8px 24px;
          border: 1px solid $primary-color;
          color: #fff;
          text-transform: uppercase;
          font-weight: 600;
          background-color: $primary-color;
      }
  }
}

</style>