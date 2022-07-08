<template>
  <div>
    <form class="container mx-auto w-6/12" action="">
        <div class="mb-6">
            <label for="username-success" class="block mb-2 text-md font-medium">Name</label>
            <input type="text" class="border border-2 text-sm block w-full p-2.5" required>
            <p class="hidden mt-2 text-sm text-green-600 dark:text-green-500"><span class="font-medium">Alright!</span> Username available!</p>
        </div>
        <div>
            <label for="username-error" class="block mb-2 text-md font-medium">Email</label>
            <input type="email" class="border border-2 text-sm block w-full p-2.5 " required>
            <p class="hidden mt-2 text-sm text-red-600 dark:text-red-500"><span class="font-medium">Oops!</span> Username already taken!</p>
        </div>
        <div>
        <label for="message" class="block mb-2 text-md font-medium mt-5">Message</label>
        <textarea id="message" rows="4" class="block p-2.5 w-full text-sm border border-2" required></textarea>
        </div>
        <button type="submit" class="w-full bg-sky-300 p-2 mt-5 uppercase font-bold hover:bg-sky-800 hover:text-white">submit</button>
    </form>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>