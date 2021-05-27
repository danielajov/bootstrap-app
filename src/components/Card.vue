<template>
  <div>
    <b-col>
      <b-card
        :title="name"
        img-src="https://mspoweruser.com/wp-content/uploads/2019/11/apps.7157.14581715871239603.af8bd868-f2d2-438d-95d2-66282697a9be.jpg"
        img-alt="nature"
        img-top
        tag="article"
        style="max-width:20rem"
        class="mb-2"
        footer="Card Footer"
      >
        <b-card-text
          >Lorem ipsum dolor sit amet consectetur, adipisicing elit. Tenetur
          ullam, tempora culpa quasi ut voluptatum accusamus doloribus debitis
          odio recusandae perspiciatis laborum pariatur, harum nemo saepe natus
          ipsum fugiat! Voluptatum?
        </b-card-text>
        <b-button variant="success">
          Apply
        </b-button>
      </b-card>
    </b-col>
  </div>
</template>

<script>
export default {
  props: ['name', 'header', 'id'],
  computed: {
    modalId() {
      return `modal-${this.id}`;
    },
  },
};
</script>

<style scoped></style>
