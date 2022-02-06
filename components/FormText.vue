<template>
    <component :is="tag" :class="['text', `text-color--${color}`, `${classes}`, top ? `margin-top--${top}` : false , bottom ? `margin-bottom--${bottom}` : false , left ? `margin-left--${left}` : false , right ? `margin-right--${right}` : false ]">
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
        classes: { type: String, default: ""},
        top : {type: String},
        bottom : {type: String},
        left : {type: String},
        right : {type: String},
        
        //type: { type: String },
    },
    computed: {
        
    }
}
</script>