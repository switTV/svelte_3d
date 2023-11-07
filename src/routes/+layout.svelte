<script lang="ts">
    import type { LayoutData } from './$types';
    
    export let data: LayoutData;
</script>

<div class="scene">
    <slot/>
</div>

<style>
    :global(*){
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    .scene {
        width: 100%;
        height: 100vh;
        position: absolute;
        background-image: radial-gradient(circle, #110d5e, #0f1d69, #0e2a72, #12377b, #1a4483);
        background-attachment: fixed;
    }
</style>