<script>
    import CurrentSeriesComponent from './CurrentSeriesComponent.vue';
    export default {
        components: {
            CurrentSeriesComponent
        }
    }
</script>
<template>
    <main>
        <section id="jumbo"></section>
        <section id="content">
            <div class="container">
                <div class="tag">CURRENT SERIES</div>
                <CurrentSeriesComponent />
                <button type="button" class="load-more">LOAD MORE</button>
            </div>
        </section>
    </main>
</template>
<style lang="scss" scoped>
    @use '../assets/style/base/common' as *;
    @use '../assets/style/abstracts/variables' as *;

    #jumbo {
        background-image: url(./../assets/img/jumbotron.jpg);
        height: 25rem;
    }

    #content {
        background-color: #1c1c1c
    }
    .container {
        @include container;
        position: relative;
        left: 0;
        top: -1.875rem;
        .tag{
            background-color: $primary-color;
            width: max-content;
            padding: .9375rem 1.25rem;
            font-weight: 600;
            font-size: 1.375rem;
        }
        .load-more {
            display: block;
            background-color: $primary-color;
            color: #FFF;
            padding: .9375rem 3.75rem;
            font-weight: 600;
            font-size: 1rem;
            border: none;
            margin: auto;
            cursor: pointer;

            &:hover{
                background-color: adjust-color($primary-color, $blackness: 30%);
            }
        }
    }

</style>