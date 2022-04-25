<template>
    <div>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Magni consectetur adipisci quod iure repellendus temporibus a! Molestiae nam modi nemo et tenetur! Culpa expedita a vitae, consequatur provident repellat quo.</p>
        <p>{{ text }}</p>
    </div>
</template>

<script>
export default {
    data() {
        return {
            text: "Hello Vue!"
        }
    }
}
</script>

<style>
    p {
        color: aqua;
    }
</style>