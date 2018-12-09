<template>
        <li v-for="book in books">{{book.title}}:{{book.author}}</li>
</template>

<script>
export default {
  name: 'BookList',
  data() {
    return {
      name: 'BookItem',
      props: ['book']
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

li {
    display: block;
    margin: 0 10px;
}
</style>
