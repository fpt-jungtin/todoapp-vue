<template>
    <tr>
      <th scope="row">1</th>
      <td>
        Todo :
        <a href="javascript:void(0)" 
          @click="triggerTaskModal"
          class="heading-todo-title trigger-task-modal">
          {{ todo.title }}
        </a>
      </td>
      <td>{{ hasTasks ? todo.tasks.length : 0 }}</td>
    </tr>
</template>

<script>
import $ from "jquery"
import 'bootstrap/dist/js/bootstrap.min.js';

export default {
  props: {
    todo: {
      type: Object,
      required: true
    }
  },
  methods: {
    triggerTaskModal() {
      this.$store.dispatch("modal/changeTodo", this.todo.id);
      
      $(document).ready(function() {
        $('#task-modal').modal('show');
      });
    }
  },
  computed: {
    hasTasks() {
      return this.todo.tasks !== null && this.todo.tasks.length > 0;
    }
  }
};
</script>

<style>
</style>