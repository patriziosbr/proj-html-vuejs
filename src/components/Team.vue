<template>
  <section class="container-fluid bg-white">
    <div class="container d-flex justify-content-space-between">
        <div class="mainHeading">
            <h5 class="text-uppercase my-4" >we like what we do</h5>
            <h2 class="my-4"><span>Team</span>of Expert</h2>
            <p class="my-4">Ethic an integrity are the bases on which our professionals build their careers.
            They are foundamentals that become daily attitudes.
            </p>
            <div class="team-photos ">
                <div class="photo d-flex mb-4">
                    <div class="images">
                        <img src="../assets/images/team-1.jpg" alt="">
                    </div>
                    <div class="txt-photo p-4">
                        <h4>David Cooper</h4>
                        <p class="text-uppercase">cto &amp; co-founder</p>
                        <div class="social-contact d-flex">
                            <div>
                                <i class="fab fa-facebook-f"></i>
                            </div>
                            <div>
                                <i class="fab fa-twitter"></i>
                            </div>
                            <div>
                                <i class="fab fa-linkedin-in"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="photo d-flex mb-4">
                    <div class="images">
                        <img src="../assets/images/team-3.jpg" alt="">
                    </div>
                    <div class="txt-photo p-4">
                        <h4>David Cooper</h4>
                        <p class="text-uppercase">cto &amp; co-founder</p>
                        <div class="social-contact d-flex">
                            <div>
                                <i class="fab fa-facebook-f"></i>
                            </div>
                            <div>
                                <i class="fab fa-twitter"></i>
                            </div>
                            <div>
                                <i class="fab fa-linkedin-in"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="photo d-flex mb-4">
                    <div class="images">
                        <img src="../assets/images/team-2.jpg" alt="">
                    </div>
                    <div class="txt-photo p-4">
                        <h4>David Cooper</h4>
                        <p class="text-uppercase">cto &amp; co-founder</p>
                        <div class="social-contact d-flex">
                            <div>
                                <i class="fab fa-facebook-f"></i>
                            </div>
                            <div>
                                <i class="fab fa-twitter"></i>
                            </div>
                            <div>
                                <i class="fab fa-linkedin-in"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="photo d-flex mb-4">
                    <div class="images">
                        <img src="../assets/images/team-4.jpg" alt="">
                    </div>
                    <div class="txt-photo p-4">
                        <h4>David Cooper</h4>
                        <p class="text-uppercase">cto &amp; co-founder</p>
                        <div class="social-contact d-flex">
                            <div>
                                <i class="fab fa-facebook-f"></i>
                            </div>
                            <div>
                                <i class="fab fa-twitter"></i>
                            </div>
                            <div>
                                <i class="fab fa-linkedin-in"></i>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
          <div class="bg-myprimary ">
              <h3>President speech</h3>
              <div class="d-flex flex-column justify-content-between">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    </p>
                    <p>
                    Autem veritatis repellendus, cum omnis, corrupti animi dicta maxime consequuntur iusto magnam eos illum esse dignissimos libero ullam molestiae doloribus corporis voluptates!
                    </p>
                    <p>
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit. Deserunt quasi delectus corporis facere provident veritatis? Eum fugit sit dolore debitis.
                    </p>
                    <p>
                        <strong>Done Joe</strong>
                    </p>
                </div>
          </div>
      </div>
  </section>
</template>

<script>
export default {
    name: "Team"
}
</script>

<style lang="scss" scoped>
@import "../style/vars.scss";
 .bg-white{
        background-color: #fff;
        padding: 64px;
        .mainHeading {
            width: 60%;
            padding: 0 32px;
            h5 {
                font-size: 16px;
                color: $primary-color;
                font-weight: 700;
            }
            h2 {
                font-size: 52px;
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
                font-size: 16px;
                line-height: 150%;
                color: #7D878E;
            }
            .team-photos {
                
                width: 100%;
                display: flex;
                justify-content: space-between;
                flex-wrap: wrap;
                .photo {
                    
                    height: 150px;
                    width: 48%;
                    .images {
                        img {
                            height:  100%;
                            border-radius: 10px;
                        }

                    }
                    .txt-photo {
                        p {
                            font-size: 13px;
                        }
                        .social-contact {
                            div {
                                display: flex;
                                align-items: center;
                                justify-content: center;
                                color: $primary-color;
                                background-color: $primary-light;
                                height: 35px;
                                width: 35px;
                                margin-right: 16px; 
                                padding: 2px;
                                border-radius: 50%;
                                cursor: pointer;
                            }
                        }
                    }
                }
            }
        }
        .bg-myprimary {
            align-self: center;
            width: 30%;
            background-color: $primary-color;
            border-radius: 20px;
            padding: 24px;
            color: #fff;
            p {
                color: #ccc;
                strong {
                    color: #fff;
                }
            }
        }
 }
//thjis is a comment
</style>