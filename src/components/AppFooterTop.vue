<script>
  export default {
    name: 'AppFooterTop'
  }
</script>

<template>
  <div id="footer-top">
    <div class="footer-top container">
        <nav class="row">
            <div class="col">
                <ul>
                <h4>DC COMICS</h4>
                <li><a href="#">Character</a></li>
                <li><a href="#">Character</a></li>
                <li><a href="#">Character</a></li>
                <li><a href="#">Character</a></li>
                <li><a href="#">Character</a></li>
                <li><a href="#">Character</a></li>
                <li><a href="#">Character</a></li>
            </ul>
            <ul>
                <h4>DC COMICS</h4>
                <li><a href="#">Character</a></li>
                <li><a href="#">Character</a></li>
            </ul>
            </div>
            <div class="col"><ul>
                <h4>DC COMICS</h4>
                <li><a href="#">Character</a></li>
                <li><a href="#">Character</a></li>
                <li><a href="#">Character</a></li>
                <li><a href="#">Character</a></li>
                <li><a href="#">Character</a></li>
                <li><a href="#">Character</a></li>
                <li><a href="#">Character</a></li>
                <li><a href="#">Character</a></li>
                <li><a href="#">Character</a></li>
                <li><a href="#">Character</a></li>
                <li><a href="#">Character</a></li>
            </ul></div>
            <div class="col"><ul>
                <h4>DC COMICS</h4>
                <li><a href="#">Character</a></li>
                <li><a href="#">Character</a></li>
                <li><a href="#">Character</a></li>
                <li><a href="#">Character</a></li>
            </ul></div>
        </nav>
        <img src="../assets/images/dc-logo-bg.png" alt="">
    </div>
  </div>
</template>

<style scoped>
    .container {
        max-width: 1200px;
        margin: 0 auto;
    } 

    #footer-top {
        padding: 2rem 0;
        background-image: url(../assets/images/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
    }

    .footer-top {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    img {
        width: 30%;
    }

    .row {
        display: flex;
        align-items: baseline;

        h4 {
            font-size: 1.1rem;
        }

        a {
            font-size: .9rem;
            color: #959595;
        }
    }


</style>