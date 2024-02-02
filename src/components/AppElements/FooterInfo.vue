<script>
  
  export default {
    name: 'FooterInfo',
    props: {
        footerTopList: Array
    }
  }
</script>

<template>
  <div class="col" v-for="(element, i) in footerTopList" :key="i">
        <ul v-for="(list, i) in element.list" :key="i">
            <h4>{{ list.heading }}</h4>
            <li v-for="(item, i) in list.listItems" :key="i"><a href="#">{{ item }}</a></li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
  h4 {
        font-size: 1.1rem;
        text-transform: uppercase;
        margin: .8rem 0;
    }

    li {
        padding: .1rem 0;
    }

    a {
        font-size: .8rem;
        color: #959595;
    }
</style>