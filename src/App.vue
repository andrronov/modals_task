<template>
  <div class="wrapper">
    <textComponent class="a-butt"></textComponent>
    <modalForm class="b-butt"></modalForm>
  </div>
</template>

<script>
import modalForm from "@/components/tryComponent.vue";
import textComponent from "@/components/textComponent.vue";

export default {
name: "App",
  components: {
    modalForm,
    textComponent,
  }
}
</script>

<style>
.wrapper{
  width: 100%;
}

body{
  display: flex;
  flex-direction: row;
  width: 100%;
  height: 100%;
  justify-content: center;
  align-items: center;
}
.a-butt{
  position: absolute;
  top: 50%;
  left: 30%;
}
.b-butt{
  position: absolute;
  top: 50%;
  right: 30%;
}
.wr_forma{
  padding: 15px;
  background-color: rgba(151, 151, 151, 0.619);
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  min-height: 90%;
}
.input_num::-webkit-outer-spin-button,
.input_num::-webkit-inner-spin-button {
   -webkit-appearance: none;
}
.btn_sub{
  padding: 5px;
  background-color: rgb(255, 180, 180);
  border: 0px;
  border-radius: 5px;
}
.btn_sub:hover{
  cursor: pointer;
  background-color: rgb(255, 118, 118);
}

.error_log{
  display: block;
  color: red;
}
._unvisible{
  display: none;
}
.success_order{
  margin-top: 10px;
  color: green;
}
</style>