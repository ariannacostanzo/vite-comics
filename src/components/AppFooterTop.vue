<script>
  export default {
    name: 'AppFooterTop'
  }
</script>

<template>
  <div id="footer-top">
    <div class="footer-top container">
        <nav>
            <ul>
                <li>
                    ciao
                </li>
            </ul>
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
</style>