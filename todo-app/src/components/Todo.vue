<template>
  <div class="ui centered card">
    <div class="content">
      <div class="header">
        {{ todo.title }}
      </div>
      <div class="meta">
        {{ todo.project }}
      </div>
      <div class="extra content">
        <span class="right floated edit icon"></span>
        <i class="edit icon"></i>
      </div>
    </div>
    <div class="ui bottom attached green basic button" v-show="todo.done">Completed</div>
    <div class="ui bottom attached red basic button" v-shwow="!todo.done">Complete</div>
  </div>
</template>

<script>
  export default {
  props: ['todo']
  };
</script>
