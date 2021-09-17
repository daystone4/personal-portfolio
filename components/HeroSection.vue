<template>
    <main id="main">
        <section class="hero">
            <h1 class="hero__title">David Stone</h1>
            <h1 class="hero__subtitle">Software Developer</h1>
            <p class="hero__text">
                You've found my tiny section on the internet. I'm currently making the transition from the world of college sports into the tech space as a developer. View a few of my projects below.
            </p>
        </section>
    </main>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.hero {
    margin: 3rem 0 0; 
    text-align: center; 

    & > * {
        margin-bottom: 1rem;
    }


    &__title {
        font-size: clamp(3.5rem, 5vw + 1rem, 5rem);
    }

    &__subtitle {
        font-size: clamp(2rem, 3vw, 2.5rem);
        opacity: 0.4;
    }

    &__text {
        font-size: clamp(1rem, 1vw + 1rem, 1.25rem);
        line-height: 1.6rem;
    }
}
</style>