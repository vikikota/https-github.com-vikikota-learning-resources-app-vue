<template>
  <ul>
    <learning-source
      v-for="resource in storedResources"
      :key="resource.id"
      :id="resource.id"
      :title="resource.title"
      :description="resource.description"
      :link="resource.link"
    >
    </learning-source>
  </ul>
</template>

<script>
import LearningSource from './LearningSource.vue';

export default {
  components: { LearningSource },
  data() {
    return {

    }
  },
  inject: ['storedResources'],
};
</script>

<style scoped>
ul {
  list-style: none;
  margin: 0;
  padding: 0;
  margin: auto;
  max-width: 40rem;
}
</style>
