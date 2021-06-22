<template>
  <section class="container">
    <nav class="navBar">
        <div class="logo">
            <a href="/">
                <img src="../assets/images/logo.svg" alt="">
            </a>
        </div>

        <div>
            <ul>
                <li v-for="(link, index) in links" :key="index">
                    <a href="#">
                        {{ link.txt }}
                    </a>
                    <a href="">
                        <i :class="(link.txt) ? '' : 'far fa-user' "></i>
                    </a>
                </li>
            </ul>
        </div>
    </nav>
  </section>
</template>

<script>
export default {
    name: "NavBar",
    props: [ "links" ]

}
</script>

<style lang="scss" scoped>
@import "../style/vars.scss";

.navBar {
    display: flex;
    justify-content: space-between;
    padding: 24px 0;

    .logo {
        width: 160px;
        img {
            width: 100%;
        }
    }

    ul {
        list-style: none;
        display: flex;
        
        li {
            padding: 8px 16px;
            text-transform: uppercase;
            a {
                text-decoration: none;
                color: #ccc;
                font-weight: 600;
            }
        }
        li:hover a {
            color: $primary-color;
        }
        li:last-child:hover a {
            color: #fff;
        }
        li:last-child {
            background-color: $primary-color;
            border-radius: 5px;
        }
    }
}

</style>