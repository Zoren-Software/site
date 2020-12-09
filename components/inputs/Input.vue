<template>
  <input class="form-input" v-model="value" :required="required" type="type">
</template>

<script>
export default {
  props: {
    initialValue: {
      type: String | Number,
    },
    required: {
      type:Boolean
    },
    placeholder: {
      type: String
    },
    type: {
      required: true,
      type: String
    }
  },
  data() {
    return {
      value: this.initialValue
    }
  },
}
</script>
