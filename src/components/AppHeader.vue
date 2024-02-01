<script>
  export default {
    name: 'AppHeader'
  }
</script>

<template>
    <header>
        <div class="header container">
            <figure>
                <img src="../assets/images/dc-logo.png" alt="">
            </figure>
            <nav>
                <ul>
                    <li><a href="#">Characters</a></li>
                    <li><a href="#">Comics</a></li>
                    <li><a href="#">Movies</a></li>
                    <li><a href="#">TV</a></li>
                    <li><a href="#">Games</a></li>
                    <li><a href="#">Collectibles</a></li>
                    <li><a href="#">Videos</a></li>
                    <li><a href="#">Fans</a></li>
                    <li><a href="#">News</a></li>
                    <li><a href="#">Shop</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>
.container {
    max-width: 1200px;
    margin: 0 auto;
    
} 

header {
    background-color: white;
}

.header {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

img {
    width: 80%;
}

ul{
    display: flex;
    gap: 35px;

    a {
        text-transform: uppercase;
        font-size: .9rem;
        font-weight: 500;
        font-family: 'Open Sans', sans-serif;
    }

}
</style>