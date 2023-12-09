<script>
export default {
    name: 'ButtonFooter',
};
</script>

<template>
    <a href="">
        <div class="button">
            sign-up now!
        </div>
    </a>
</template>


<style scoped lang="scss">
@use '../../styles/partials/variables.scss' as *;

a {
    text-decoration: none;
    color: $primary;

    .button {
        width: 140px;
        height: 50px;
        border: 1px solid $onhover;
        display: flex;
        align-items: center;
        justify-content: center;
        text-transform: uppercase;

        &:hover {
            color: $onhover;
            border: 1px solid $primary;
        }
    }
}
</style>