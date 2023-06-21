<template>
  <li :class="linkClass">
    <router-link :to=link>{{ text }}<slot></slot></router-link>
  </li>
</template>
<script>
export default {
    props: {
        link: {
            required: true,
            type: String,
        },
        text: {
            required: false,
            type: String,
        },
        linkClass: {
            required:  true,
            type: String,
        }
    },
}
</script>
