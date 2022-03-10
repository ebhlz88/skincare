<template>
  <router-view />
</template>
<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "App",
});
</script>
<style>
@font-face {
  font-family: SFpro;
  src: url("./assets/sfpro.ttf");
}
* {
  font-family: SFpro;
  letter-spacing: 0.5px;
}
.flex-row {
  display: flex;
  flex-direction: row;
}
.flex-column {
  display: flex;
  flex-direction: column;
}
.center {
  justify-content: center;
  align-items: center;
}
.colorwhite {
  color: white;
}
.colorblack {
  color: black;
}
.colorblue {
  color: #334acb;
}
button {
  border: none;
  border-radius: 10px;
}
button:hover {
  cursor: pointer;
}
.toleft {
  align-items: flex-end;
}
.heading2 {
  font-size: 21px;
  font-weight: 700;
  text-transform: uppercase;
}
.heading3 {
  font-size: 11px;
  font-weight: 700;
  text-transform: uppercase;
}
.spacebtw {
  justify-content: space-between;
}
</style>
