<template>
  <div :class="color">
    <p>
      <slot>{{message}}</slot>
    </p>
  </div>
  <!-- warning info success  -->
</template>

<script>
export default {
  name: "DaoNote",
  props: {
    message: {
      type: String,
      default: ""
    },
    color: {
      type: String,
      default: "info"
    }
  }
};
</script>

<style>
div {
  margin-bottom: 15px;
  padding: 4px 12px;
}

.danger {
  background-color: #ffdddd;
  border-left: 6px solid #f44336;
}

.success {
  background-color: #ddffdd;
  border-left: 6px solid #4caf50;
}

.info {
  background-color: #e7f3fe;
  border-left: 6px solid #2196f3;
}

.warning {
  background-color: #ffffcc;
  border-left: 6px solid #ffeb3b;
}
</style>