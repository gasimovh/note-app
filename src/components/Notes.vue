<template>
  <div>
    <div class="notes">
      <div v-for="note in allNotes" :key="note.id" class="note">
        <div class="nav">
          <div class="title">{{ note.title }}</div>
          <div class="edit">
            <button>
              <img src="../assets/edit.png" alt="" />
            </button>
          </div>
          <div class="delete">
            <button>
              <img src="../assets/trash.png" alt="" />
            </button>
          </div>
        </div>
        <div class="body">
          <div class="text">
            {{ note.text }}
          </div>
          <div class="date">{{ note.date }}</div>
        </div>
        <div class="bottom">
          <button>
            <img src="../assets/facebook.png" alt="" />
          </button>
          <button>
            <img src="../assets/twitter.png" alt="" />
          </button>
          <button>
            <img src="../assets/file.png" alt="" />
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      allNotes: [
        {
          title: "Title 1",
          text: "Lorem ipsum dolor, sit amet consectetur adipisicing elit. In repudiandae id perferendis, officiis vero distinctio eligendi minus culpa. Sit, excepturi! Ipsa vel vero, aspernatur alias minus, reprehenderit quae sequi perspiciatis a rem iure aliquam. Exercitationem iste sed rem assumenda tempore possimus, totam vel. Adipisci cupiditate commodi aliquam reiciendis ipsum deserunt?",
          date: "21 August 2021",
        },
        {
          title: "Title 2",
          text: "Lorem ipsum dolor, sit amet consectetur adipisicing elit. In repudiandae id perferendis, officiis vero distinctio eligendi minus culpa. Sit, excepturi! Ipsa vel vero, aspernatur alias minus, reprehenderit quae sequi perspiciatis a rem iure aliquam. Exercitationem iste sed rem assumenda tempore possimus, totam vel. Adipisci cupiditate commodi aliquam reiciendis ipsum deserunt?",
          date: "21 August 2021",
        },
        {
          title: "Title 3",
          text: "Lorem ipsum dolor, sit amet consectetur adipisicing elit. In repudiandae id perferendis, officiis vero distinctio eligendi minus culpa. Sit, excepturi! Ipsa vel vero, aspernatur alias minus, reprehenderit quae sequi perspiciatis a rem iure aliquam. Exercitationem iste sed rem assumenda tempore possimus, totam vel. Adipisci cupiditate commodi aliquam reiciendis ipsum deserunt?",
          date: "21 August 2021",
        },
        {
          title: "Title 4",
          text: "Lorem ipsum dolor, sit amet consectetur adipisicing elit. In repudiandae id perferendis, officiis vero distinctio eligendi minus culpa. Sit, excepturi! Ipsa vel vero, aspernatur alias minus, reprehenderit quae sequi perspiciatis a rem iure aliquam. Exercitationem iste sed rem assumenda tempore possimus, totam vel. Adipisci cupiditate commodi aliquam reiciendis ipsum deserunt?",
          date: "21 August 2021",
        },
        {
          title: "Title 5",
          text: "Lorem ipsum dolor, sit amet consectetur adipisicing elit. In repudiandae id perferendis, officiis vero distinctio eligendi minus culpa. Sit, excepturi! Ipsa vel vero, aspernatur alias minus, reprehenderit quae sequi perspiciatis a rem iure aliquam. Exercitationem iste sed rem assumenda tempore possimus, totam vel. Adipisci cupiditate commodi aliquam reiciendis ipsum deserunt?",
          date: "21 August 2021",
        },
        {
          title: "Title 6",
          text: "Lorem ipsum dolor, sit amet consectetur adipisicing elit. In repudiandae id perferendis, officiis vero distinctio eligendi minus culpa. Sit, excepturi! Ipsa vel vero, aspernatur alias minus, reprehenderit quae sequi perspiciatis a rem iure aliquam. Exercitationem iste sed rem assumenda tempore possimus, totam vel. Adipisci cupiditate commodi aliquam reiciendis ipsum deserunt?",
          date: "21 August 2021",
        },
      ],
    };
  },
};
</script>

<style scoped>
.notes {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-gap: 1rem;
  font-weight: 300;
}

.title {
  padding-top: 10px;
  flex-basis: 100%;
  font-weight: 600;
}
.nav {
  display: flex;
  flex-direction: start;
  margin-bottom: 10px;
}

.nav > * + * {
  margin-right: 10px;
}

.note {
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 0px 16px 0 rgba(0, 0, 0, 0.2);
}

.date {
  margin: 10px auto;
  font-weight: 600;
  font-size: 14px;
  display: flex;
  justify-content: flex-end;
}

img {
  width: 20px;
  height: 20px;
}

.bottom {
  display: flex;
  justify-content: flex-end;
}
.bottom > * {
  margin-right: 10px;
}

@media (min-width: 500px) {
  .notes {
    grid-template-columns: 1fr;
  }
}

@media (min-width: 900px) {
  .notes {
    grid-template-columns: 1fr;
    grid-template-columns: repeat(3, 1fr);
  }
}
</style>