<template>
<div>
    <Header/>

<main class="flex">
  <!-- Sidebar -->
     <div class="py-5 px-8 border-r-2 border-gray-300 w-2/12">
        <Sidebar/>
     </div>

<!-- Content -->
      <div class="py-5 px-8 w-10/12">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatum iure cupiditate adipisci accusamus? Necessitatibus adipisci reprehenderit tenetur molestiae quos quo molestias, doloremque a! A sequi perspiciatis quidem dolor beatae, neque necessitatibus corrupti, vero impedit officiis enim rem accusantium quibusdam quos porro iste voluptates quisquam! Ducimus quisquam laudantium corrupti rem. Vel.
      </div>
</main>

</div>
</template>

<script>
import Header from '../components/Header.vue'
export default {
  components: { Header },
  name: 'IndexPage'
}
</script>
