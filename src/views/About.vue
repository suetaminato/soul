<template>
  <div class="home">
    <h1>About!</h1>
    <div class="button-list">
      <Button msg="Entrar" isNeutral/>
      <Button msg="Ainda não tenho conta" isAlert/>
    </div> 
  </div>
</template>

<script>
// @ is an alias to /src
import Button from '@/components/Button.vue'

export default {
  name: 'home',
  components: {
    Button
  }
}
</script>

<style>

</style>
