<template>
  <section class="language">
    <plateTitle :title1="commonData.title[19]" :title2="commonData.title[20]" />
    <figure class="footer-qr">
      <img src="static/jackli_qr.png" alt="ooJacklioO" class="qr-img visible-print" />
    </figure>
  </section>
</template>

<script>
import plateTitle from "./PlateTitle"
import data from "./data.json"
export default {
   components: { plateTitle },
   data() {
    return {
      commonData: data.CommonData
    }
}};
</script>

<style>
</style>

