<template>
  <div class="container">
    <form class="create-note-form">
      <div class="title">
        <input type="text" placeholder="Title" />
      </div>
      <div class="note">
        <textarea type="text" placeholder="Take a note..." />
      </div>
      <div class="save">
        <button>
          <img src="../assets/save.png" alt="" />
        </button>
      </div>
    </form>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.create-note-form {
  /* margin-left: 100px;
  margin-top: 50px; */
  width: 400px;
  height: 300px;
  padding: 15px 20px 0px 20px;
  border-radius: 10px;
  box-shadow: 0 0px 16px 0 rgba(0, 0, 0, 0.2);
  display: flex;
  flex-direction: column;
}

.note {
  margin-top: 10px;
  margin-bottom: 10px;
  flex-basis: 100%;
}

img {
  width: 20px;
  height: 21px;
}
.save {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  /* margin-right: 10px; */
  margin-bottom: 10px;
}

input {
  font-weight: 600;
}

input,
textarea {
  border-top-style: hidden;
  border-right-style: hidden;
  border-left-style: hidden;
  border-bottom-style: hidden;
  width: 100%;
  height: 100%;
  resize: none;
}

*:focus {
  outline: none;
}
</style>