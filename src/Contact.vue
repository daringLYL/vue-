<template>
  <section class="language">
    <PlateTitle :title1="commonData.title.plateTitle[8]" :title2="commonData.title.plateTitle[9]" />
    <figure class="footer-qr">
      <img src="static/jackli_qr.png" alt="ooJacklioO" class="qr-img visible-print" />
    </figure>
  </section>
</template>

<script>
import PlateTitle from "./PlateTitle"
import data from "./data.json"
export default {
   components: { PlateTitle },
   data() {
    return {
      commonData: data.CommonData
    }
}};
</script>

<style>
</style>
