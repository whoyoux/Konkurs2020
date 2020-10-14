<template>
  <div id="wrapper" class="max-w-xl px-4 py-4 mx-auto">
            <div class="sm:grid sm:h-32 sm:grid-flow-row sm:gap-4 sm:grid-cols-3">
                <div id="jh-stats-positive" class="flex flex-col justify-center px-4 py-4 bg-white border border-gray-300 rounded">
                    <div>
                        <p class="text-3xl font-semibold text-center text-yellow-600">{{newSick}}</p>
                        <p class="text-lg text-center text-gray-500">{{all ? "Zachorowania" : "Nowe zachorowania"}}</p>
                    </div>
                </div>
    
                <div id="jh-stats-negative" class="flex flex-col justify-center px-4 py-4 mt-4 bg-white border border-gray-300 rounded sm:mt-0">
                    <div>
                        <p class="text-3xl font-semibold text-center text-green-700">{{newRecovery}}</p>
                        <p class="text-lg text-center text-gray-500">Wyzdrowienia</p>
                    </div>
                </div>

                <div id="jh-stats-neutral" class="flex flex-col justify-center px-4 py-4 mt-4 bg-white border border-gray-300 rounded sm:mt-0">
                    <div>
                        <p class="text-3xl font-semibold text-center text-red-800">{{newDeads}}</p>
                        <p class="text-lg text-center text-gray-500">Zgony</p>
                    </div>
                </div>
            </div>
        </div>
</template>

<script>
export default {
    name: 'Stats',
    props: {
        newSick: String,
        newRecovery: String,
        newDeads: String,
        all: Boolean
    }
}
</script>

<style>

</style>