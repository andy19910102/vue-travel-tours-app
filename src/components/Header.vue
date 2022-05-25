<template>
  <header class="jumbotron">
    <div class="container">
      <h1>{{ title }}</h1>
      <p class="lead">{{ subtitle }}</p>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  props: ["title", "subtitle", "thumbnail"],
};
</script>