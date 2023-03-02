<template>
    <li class="header-list-items">
        <a :href="menu.link">
            {{menu.label}}
        </a>
    </li>
</template>

<script>
    export default {

        props:{

            menu:{
                type: Object,
                required: true
            }
        }
    }
</script>

<style lang="scss" scoped>
    @use '../style/partials/variables' as *;
.header-list-items{
    position: relative;

    &:hover{
      color: $main-blue;
    }

    &:hover::after{
      content: '';
      display: block;
      width: 40px;
      padding: 2px;
      background-color: $main-blue;
      position: absolute;
      top: 60px;
      left: 50%;
      transform: translateX(-50%);
    }
  }
</style>