<template>
    <li>
    <div class="flex">
    <div class="flex-shrink-0">
        <div class="flex items-center justify-center h-12 w-12 rounded-md bg-red-500 text-white">
        <!-- Heroicon name: globe-alt -->
        <!-- <svg class="h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 12a9 9 0 01-9 9m9-9a9 9 0 00-9-9m9 9H3m9 9a9 9 0 01-9-9m9 9c1.657 0 3-4.03 3-9s-1.343-9-3-9m0 18c-1.657 0-3-4.03-3-9s1.343-9 3-9m-9 9a9 9 0 019-9" />
        </svg> -->
        <!-- LINK DO TEGO -->
        <!-- https://www.iconpacks.net/free-icon/medical-mask-3974.html -->
            <img :src="require(`@/assets/img/${imgName}`)" :alt="`${imgName}`" style="width: 70%; height: 70%">
        </div>
    </div>
    <div class="ml-4">
        <h4 class="text-lg leading-6 font-medium text-gray-900">{{title}}</h4>
        <p class="mt-2 text-base leading-6 text-gray-500">
            {{desc}}
        </p>
    </div>
    </div>
    </li>
</template>

<script>
export default {
    name: "PreventionListItem",
    props: {
        imgName: String,
        title: String,
        desc: String
    }
}
</script>

<style>

</style>