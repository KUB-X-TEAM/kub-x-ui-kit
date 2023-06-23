<template>
  <div id="app">
    <KButton arrow="true" size="small">your mummy love me long time</KButton>
    <KButton arrow="true">your mummy love me long time</KButton>
    <KButton arrow="true" size="big">your mummy love me long time</KButton>
    <br>
    <KButton color="secondary" href="https://kubx.cc" size="small">your mummy love me long time</KButton>
    <KButton color="secondary" href="https://kubx.cc">your mummy love me long time</KButton>
    <KButton color="secondary" href="https://kubx.cc" size="big">your mummy love me long time</KButton>
    <br>
    <KForm>
      <KInputText></KInputText>
      <KButton size="small">Send</KButton>
    </KForm>
  </div>
</template>

<script>
import KButton from "@/components/Buttons/KButton.vue";
import KForm from "@/components/KForm.vue";
import KInputText from "@/components/Inputs/KInputText.vue";
export default {
  name: 'App',
  components: {
    KButton,
    KForm,
    KInputText
  }
}
</script>

<style>
body {
  background-color: #1E1E1E;
}
</style>
