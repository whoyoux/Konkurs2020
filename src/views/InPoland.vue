<template>
  <div class="py-12 bg-white">
    <div class="max-w-screen-xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="lg:text-center">
        <h3 class="mt-2 text-center text-3xl leading-8 font-bold tracking-tight text-gray-900 sm:text-4xl sm:leading-10">
          Liczba zakażen w Polsce od wczoraj
        </h3>
      <p class="mt-4 max-w-2xl text-xl leading-7 text-gray-500 lg:mx-auto">
        
      </p>
      <Stats 
        :newSick="`${new_sick}`"
        :newRecovery="`${new_recovery}`"
        :newDeads="`${new_deads}`"
      />
    </div>
  </div>
</div>
</template>

<script>
import Stats from '@/components/Stats.vue'
import axios from 'axios';
export default {
  name: 'InPoland',
  components: {
    Stats
  },
  data() {
    return {
      new_sick: "",
      new_recovery: "",
      new_deads: ""
    }
  },
  async mounted() {
    try {
      const response = await axios.get("https://coronavirus-19-api.herokuapp.com/countries/Poland");
      const data = response.data;
      this.new_sick = data.todayCases;
      this.new_recovery = data.recovered;
      this.new_deads = data.todayDeaths;
    } catch(err){
      console.log(err);
    }
  }
}
</script>

<style>

</style>