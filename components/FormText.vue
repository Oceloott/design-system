<template>
    <component :is="tag" :class="['text', `text-color--${color}`, `${classes}` ]">
        {{text}}
    </component>
</template>

<script>
export default {
    name: "FormText",
    props: {
        text: String,
        tag: { type : String, default: "h1"},
        color: { type: String, default: "black"},
        classes: { type: String, default: ""}
        //type: { type: String },
    },
    computed: {
        
    }
}
</script>