<template>
    <li class="list-hero-items">
        <a :href="comics.link">
            {{ comics.label }}
        </a>
    </li>
</template>

<script>
    export default {
        props:{

            comics:{
                type:Object,
                required: true
            }
        }
    }
</script>

