<template>
  <div class="home">
    <div class="create-note">
      <CreateNote />
    </div>
    <div class="notes">
      <Notes />
    </div>
  </div>
</template>

<script>
import CreateNote from "../components/CreateNote.vue";
import Notes from "../components/Notes.vue";

export default {
  name: "Home",
  components: {
    CreateNote,
    Notes,
  },
};
</script>

<style scoped>
.home {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  padding: 50px;
}

.notes {
  margin-top: 50px;
}
</style>
