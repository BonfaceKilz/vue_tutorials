<template>
    <div class="sourceselection">
        <h4>Select News source</h4>
        <select class="from-control" id="" v-on:change:"sourceChanged">
            <option v-bind:value="source.id" value="" v-for="source in sources">{{source.name}}</option>
        </select>
    </div>
  </template>

<script>
 
export default {
  name: 'sourceselection',
  data () {
    return {
      sources: [],
      source: ''
    }
  }
}
</script>

<style scoped>

 </style>
