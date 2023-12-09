<script>
export default {
    name: 'Jumbotronnn',
};
</script>

<template>
    <div class="jumbo">
        <div class="container">
            <ul>
                <li>ciao</li>
                <li>ciao</li>
                <li>ciao</li>
                <li>ciao</li>
                <li>ciao</li>
                <li>ciao</li>
            </ul>
        </div>
    </div>
</template>


<style scoped lang="scss">
@use '../../styles/partials/variables.scss' as *;

.jumbo {
    background-color: $onhover;
}

.container {
    width: 80%;
    height: 150px;
    margin: 0 auto;

    ul {
        list-style: none;
        display: flex;
        justify-content: space-around;
    }
}
</style>