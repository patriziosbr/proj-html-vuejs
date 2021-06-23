<template>
    <section class="container-fluid">
        <div class="container d-flex">

            <div class="mainForm ">
                <div class=" mainHeading ">
                    <h5 class="text-uppercase mb-4">newsletter</h5>
                    <h3 class="mb-4">Get in <span>Touch</span></h3>
                    <p class="my-2">We will respond your message as soon as possibile.</p>
                </div>
                <div class="formCont">
                    <form action="post">
                        <input type="text" name="name" id="name" placeholder="Name">
                        <input type="text" name="mail" id="mail" placeholder="Email">
                        <input type="phone" name="phone" id="phone" placeholder="Phone">
                        <input type="text" name="info" id="info" placeholder="More info">
                        <textarea rows="4" cols="50" name="comment" form="usrform">
                        Message</textarea>
                    <div class="btn">send</div>
                    </form>
                </div>
            </div> 

            <div class="info">
                <h2 class="mb-3">Example Inc.</h2>
                <p class="mb-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, accusantium.</p>
                <p class="mb-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, accusantium.</p>
                <div class="icons">
                    <div class="phone d-flex">
                        <div class="circle">
                            <i class="fas fa-phone-alt"></i>
                        </div>
                        <p>123456</p>
                    </div>
                    <div class="mail d-flex">
                        <div class="circle">
                            <i class="fas fa-envelope"></i>
                        </div>
                        <p>mail@mail.com</p>
                    </div>
                    <div class="location d-flex">
                        <div class="circle">
                            <i class="fas fa-map-marker-alt"></i>
                        </div>
                        <p>Maps via 123</p>
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
.mainForm {
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
            color: $heading-dark;
        span {
            color: $primary-color;
            padding: 4px 10px;
            border-radius: 5px;
            display: inline-block;
            background-color: rgba($color: $primary-color, $alpha: 0.3);
            }
        }
        p {
            font-size: 18px;
        }
    } //fine main heading
    //start form
    .formCont {
        
        display: flex;

        input {
            margin: 8px;
            padding: 16px;
            width: calc( 100% / 2 - 32px);
            background-color: $grey-form;
            border: none;
            border-radius: 5px;
        }
        textarea {
            width: calc(100% - 48px);
            margin: 8px;
            padding: 16px;
            background-color: $grey-form;
            border: none;
            border-radius: 5px;
        }
        .btn {
            margin: 8px;
            padding: 8px 24px;
            border: 1px solid $primary-color;
            color: #fff;
            text-transform: uppercase;
            font-weight: 600;
            background-color: $primary-color;
      }
    }
}
.info {
    padding: 32px;
}

</style>