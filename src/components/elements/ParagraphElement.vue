<template lang="pug">
p.paragraph(v-html="element.text")
</template>
<script lang="ts">
import { Component, Vue, Prop } from "vue-property-decorator";
import { Paragraph } from "../../shared/entities";

@Component({
  name: "ParagraphElement",
})
export default class ParagraphElement extends Vue {
  @Prop(Object) private element: Paragraph;
}

</script>
<style scoped lang="stylus"></style>
