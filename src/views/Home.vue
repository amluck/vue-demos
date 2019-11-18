<template>
  <div class="home">
    <element-form></element-form>
    <!-- <hello-element></hello-element> -->
  </div>
</template>

<script>
// @ is an alias to /src
import HelloElement from "@/components/HelloElement.vue";
import ElementForm from "@/components/ElementForm.vue";

export default {
  name: "home",
  components: {
    // HelloElement,
    ElementForm
  }
};
</script>
