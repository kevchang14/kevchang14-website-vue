<template>
    <ol>
      <!--
        Now we provide each todo-item with the todo object
        it's representing, so that its content can be dynamic.
        We also need to provide each component with a "key",
        which will be explained later.
      -->
        <li v-for="(item, index) in list" :key="index">
            {{item.text}} <b-button>I am a button </b-button>
        </li>
    </ol>
</template>

<script>
export default {
  name: 'GroceryList',
  props: {
    list: Array,
  }
}
</script>