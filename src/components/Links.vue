<template>
    <div>
    <h2>Links</h2>
    <ul>
        <li v-for="link in links" :key="link.link_name">{{link.link_name}}: 
            <a :href="link.address" v-if="'alias' in link" target="blank">{{link.alias}}</a>
            <a :href="link.address" v-else target="_blank">{{link.address}}</a>
        </li>
    </ul>
    </div>
</template>

<script>
export default {
    name: 'Links',
    props: {
        links: Array
    }
}
</script>

<style scoped>
    h2 {
        text-align: left;
    }
    ul {
        height: 10%;
        column-count: 2;
        column-gap: normal;
        -webkit-column-count: 2;
        -moz-column-count: 2;
        text-align: left;
        padding-left: 0%;
    }
    li {
        display: inline-block;
        padding-right: 10%;
    }
    a {
        color: black;
    }
    a:hover {
        color: blue;
    }
    a:click {
        color: red;
    }
</style>