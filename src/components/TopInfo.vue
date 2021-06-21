<template>
  <section>
    <div class="container-fluid topInfo-bg">

        <div class="container topInfo">

            <div class="clock">
                <i class="fas fa-clock"></i>
                <p class="special">Open Hours: Mon - Sat 9:00 - 18:00</p> 
            </div>

            <div class="rgt-info">

                <div class="mail">
                    <i class="fas fa-phone-alt"></i>
                    <p >+1(305)1234-5678</p>
                </div>

                <div class="mail">
                    <i class="fas fa-envelope"></i>
                    <p>hello@example.com</p>
                </div>

                <ul class="social">
                    
                    <li> 
                        <a href="#">
                            <i class="fab fa-facebook-f"></i>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="fab fa-twitter"></i>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="fab fa-linkedin-in"></i>
                        </a>
                    </li>
                </ul>
                
            </div>

        </div>

    </div>
  </section>
</template>

<script>
export default {
    name: "TopInfo"
}
</script>

<style lang="scss" scoped>
@import "../style/vars.scss";

    
    .topInfo-bg {
        height: 40px;
        background-color: $bg-top-head;
        font-size: 14px;
        
        .topInfo {
            color: #fff;
            display: flex;
            justify-content: space-between;
            align-items: center;

            .clock {
                display: flex;
                align-items: center;
                p.special {
                    margin: 0;
                    line-height: 40px;
                    margin-left: 8px;
                }
                
            }
            .rgt-info {
                display: flex;
                align-items: center;
                .phone,
                .mail,
                .social {
                    display: flex;
                    margin-left: 32px;
                    align-items: center;
                }
                
                    .social {
                        list-style: none;
                        margin: 0;
                        padding: 0 0 0 16px;
                        li {
                            margin: 0 16px;
                            a {
                                color: #fff;
                            }
                        }
                    }
                
                p {
                    margin: 0;
                    margin-left: 8px;
                }
                
            }
        }
        
    }

</style>