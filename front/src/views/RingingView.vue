<template>
  <div class="box">
    <div class="text">
      Zaraz nastąpi połączenie z konsultantem.
      Poszę odebrać telefon.
    </div>
    <div style="margin-left:auto; height:auto ;">
      <img v-bind:src="Gphone" />
    </div>  
  </div>
</template>

<script>
import phone from "/workspace/kurs/front/src/images/greenphone.png"

export default {
  data() {
    return {
      Gphone: phone
    }
  },
}
</script>

