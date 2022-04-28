<template>
  <div>
    <button @click="toggle">Modal</button>
    <teleport to="body">
      <div v-show="show" class="modal">
        <h1>Title</h1>
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Non ratione
          ex dolores ut quod maxime dolor quos consequatur, perferendis, harum
          nesciunt quas neque molestiae magnam repellendus similique animi
          praesentium nihil?
        </p>
        <button @click="toggle">Close</button>
      </div>
    </teleport>
  </div>
</template>

<script>
export default {
  name: "ModalItem",
  data() {
    return {
      show: false,
    };
  },
  methods: {
    toggle() {
      this.show = !this.show;
    },
  },
};
</script>
