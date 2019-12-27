<template>
  <div class="q-pa-md row items-start q-gutter-md">
    
    <q-card class="my-card">
      <q-img
        src="../assets/telegram.png"
        basic
      >
        <div class="absolute-bottom text-subtitle2 text-center">
          미세먼지 알림 봇
        </div>
      </q-img>
    </q-card>

    <q-dialog
      v-model="medium"
    >
      <q-card style="width: 700px; max-width: 80vw;">
        <q-card-section>
          <div class="text-h6">Medium</div>
        </q-card-section>

        <q-card-section>
          Click/Tap on the backdrop.
        </q-card-section>

        <q-card-actions align="right" class="bg-white text-teal">
          <q-btn flat label="OK" v-close-popup />
        </q-card-actions>
      </q-card>
    </q-dialog>

  </div>
</template>

<script>
export default {
  name: 'PageIndex',
  
  data() {
    return {
      medium: false
    }
  },


}
</script>
<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 250px
</style>