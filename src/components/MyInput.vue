<template>
    <div>
        <label>{{label}}</label>
        <input type="text" :value="value" @input="$emit('input', $event.target.value)">
        <span>Output: {{value}}</span>
    </div>
</template>
<script lang = "ts">
export default {
    props: ["label", "value"]
}
</script>