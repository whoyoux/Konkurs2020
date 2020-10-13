<template>
  <div class="py-12 bg-white">
    <div class="max-w-screen-xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="lg:text-center">
        <p class="text-base leading-6 text-red-600 font-semibold tracking-wide uppercase">Profilaktyka</p>
        <h3 class="mt-2 text-3xl leading-8 font-bold tracking-tight text-gray-900 sm:text-4xl sm:leading-10">
          Koronawirus
        </h3>
      <p class="mt-4 max-w-2xl text-xl leading-7 text-gray-500 lg:mx-auto">
        Proste kroki, które pokazują jak bezpiecznie żyć bez obawiania się zakażeniu się nim.
      </p>
    </div>

    <div class="mt-10">
      <ul class="md:grid md:grid-cols-2 md:gap-x-8 md:gap-y-10">
        <PreventionList imgName="mask.svg" title="Maseczki ochronne" desc="Maseczka znacznie utrudnia wirusowi na przedostanie się do naszego układu oddechowego."/>
        <PreventionList imgName="hands.svg" title="Mycie rąk" desc="Myj dokładnie ręcę przez przynajmniej 30 sekund."/>
        <PreventionList imgName="mask.svg" title="esssa" desc="sesdes"/>
        <PreventionList imgName="mask.svg" title="esssa" desc="sesdes"/>
        <PreventionList imgName="mask.svg" title="esssa" desc="sesdes"/>
      </ul>
    </div>
  </div>
</div>
</template>

<script>
import PreventionList from "@/components/PreventionList.vue";
export default {
    components: {
        PreventionList
    }
}
</script>

<style>

</style>