<script>
    import {
        createEventDispatcher
    } from 'svelte';
import { element } from 'svelte/internal';
    const dispatch = createEventDispatcher();
    export let items;
    export let activeItem;
     
</script>

<div class=" border-b-2 fixed w-full bg-gray-100 p-6 ">
    <div class=" w-4/12 m-auto">
        <ul class="flex justify-between">
            {#each items as item}
      <li on:click="{() => dispatch('tabChange' , item)}">
            <div class=" border-b-2  cursor-pointer font-extralight text-2xl  duration-300 transition-all hover:border-black p-2 " class:active={item === activeItem}>{item}</div>
      </li>
      {/each}
    </ul>
</div>
</div>

