<template lang="pug">
    v-dialog(v-model='openContactModal' persistent width='60%')
        v-card(color='#fff6d3' outlined flat rounded)
            v-toolbar(color='transparent' flat)
                v-btn(icon color='#eb6b6f' @click='closeContactModal()') 
                    v-icon fa-times
                h1.ml-4(style='color: #eb6b6f') Let's talk 
                v-spacer
                v-btn(icon color='#eb6b6f' @click='clearForm()') 
                    v-icon(class='fas') fa-redo
            v-card-subtitle(style='color: #7c3f58') Thank you for taking your time to reach out. How can I help you?
            v-card-text
                v-form
                    v-text-field(outlined color='#7c3f58' label='Name' v-model='name')
                    v-text-field(outlined color='#7c3f58' label='Email' v-model='email')
                    v-textarea(outlined color='#7c3f58' label='Message' v-model='message')
                    v-spacer
                    v-btn(outlined rounded color='#7c3f58') Send Message

</template>
<script>
export default {
  name: "Contact",
  props: {
    openContactModal: {
      type: Boolean,
      default: false,
    },
  },
  data() {
    return {
      name: "",
      email: "",
      message: "",
    };
  },
  methods: {
    closeContactModal: function() {
      this.$emit("update:openContactModal", false);
    },
    clearForm: function() {
      this.name = "";
      this.email = "";
      this.message = "";
    },
  },
};
</script>
<style>
.theme--light.v-text-field--outlined:not(.v-input--is-focused):not(.v-input--has-state)
  > .v-input__control
  > .v-input__slot
  fieldset {
  color: #7c3f58 !important;
}
.theme--light.v-label {
  color: #7c3f588c !important;
}
</style>
