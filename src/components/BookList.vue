<template>
    <div>
        <h1>{{title}}</h1>
        <ul>
            <li v-for="book in books">{{book.title}}: {{book.author}}</li>
        </ul>
    </div>
</template>

<script>
    export default {
        name:"BookList",
        data(){
            return{
                title: 'All Books',
                books: [
                    {title:'Book 1', author:'Sumit'},
                    {title:'Book 2', author:'John'},
                    {title:'Book 3', author:'Xyz'}
                ]
            }
        }
    }
</script>

<style scoped>
h1, h2 { 
    font-weight: normal
}
ul{
    list-style-type: none;
    padding: 0;
}
li{
    display: block;
    margin: 0 10px;
}
</style>