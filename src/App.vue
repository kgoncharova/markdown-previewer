<template>
  <div class="container">
    <div class="row mt-4">
      <div class="col text-center">
        <h1 class="text-light">Markdown Preview</h1>
      </div>
    </div>

    <div class="row mt-4">
      <div class="col-md-6">
        <h4 class="text-light">Markdown</h4>
        <textarea 
          class="info"
          v-model="markdown"
        />
      </div>
      <div class="col-md-6">
        <h4 class="text-light">Preview</h4>
        <div class="info">
          {{ markdown }}
        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      markdown: '',
    };
  },
};
</script>

<style scoped>
textarea {
  resize: none;
  border: 2px dashed orange;
  outline: none;
}
.info {
  height: 400px;
  width: 100%;
  border-radius: 5px;
  background-color: rgba(255, 255, 255, 0.9);
}
</style>
