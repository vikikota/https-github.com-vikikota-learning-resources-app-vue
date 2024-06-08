<template>
  <ul>
    <learning-source
      v-for="resource in resources"
      :key="resource.id"
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
  props: ["resources"],
  data() {
    return {

    }
  },
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
