<script>
const { bind } = require("svelte/internal")

export let height = innerHeight
export let width = innerWidth

let innerHeight, innerWidth, canvas

</script>

<svelte:window bind:innerHeight={innerHeight} bind:innerWidth={innerWidth} />

<canvas 
    bind:this={canvas} 
    height={height}
    width={width}
/>