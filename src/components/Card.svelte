<script>
    export let info
    export let image
</script>

<div class="sm:max-w-sm max-w-52 rounded overflow-hidden shadow-lg">
    <img class="w-full" src={image} alt="Sunset in the mountains">
    <div class="px-6 py-4">
      <p class="text-gray-700 text-base text-ellipsis line-clamp-2">{info}</p>
    </div>
  </div>