<template>
    <input :type="type" :name="name" :placeholder="placeholder" >
</template>

<script>
    //--text-color-primary-black
export default {
    name: "FormText",
    props: {
        placeholder: String,
        name: { type : String, default: "input"},
        type: { type : String, default: "text"},
        //classes: { type: String},
        //color: { type: String, default: "primary-black"}
    },
    computed: {
        
    }
}
</script>