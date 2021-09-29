<template>
  <div id="app-7">
    <p>Những thứ họ mua:</p>
    <ol>
      <todo-item
          v-for="item in groceryList"
          v-bind:todo="item"
          v-bind:key="item.id">
      </todo-item>
    </ol>
  </div>
</template>

<script>
import TodoItem from "@/components/todo-item";
export default {
  name: 'HelloWorld',
  components: {TodoItem},
  data() {
    return {
      groceryList: [
        { id: 0, text: 'Cà pháo' },
        { id: 1, text: 'Mắm tôm' },
        { id: 2, text: 'Miễn ăn được là được' }
      ]
    }
  }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
