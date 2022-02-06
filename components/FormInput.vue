<template>
    <input :type="type" :name="name" :placeholder="placeholder" :class='[`--text-color-${color}`, `${classes}`]'>
</template>

<script>
export default {
    name: "FormText",
    props: {
        placeholder: String,
        name: { type : String, default: "input"},
        type: { type : String, default: "text"},
        classes: { type: String, default: ""},
        color: { type: String, default: "primary-black"}
    },
    computed: {
        
    }
}
</script>