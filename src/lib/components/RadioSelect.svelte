<script>
    let { content, name, id } = $props()
</script>

<div class="relative w-fit">
    <input type="radio" name={name} id={id} class="hidden peer">
    <label for={id} class="flex gap-4 p-4 rounded-3xl bg-white bg-opacity-90 backdrop-blur-2xl shadow-xl hover:bg-opacity-75 peer-checked:bg-orange-700 peer-checked:text-white">
        <div>
            <h6 class="text-base">{content}</h6>
        </div>
    </label>
</div>