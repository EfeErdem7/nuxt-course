<template>
    <div class="Hero container">
        <div class="text-container">
            <h1 class="header">Find your Fire Extinguisher</h1>
            <p class="snippet">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Iste iusto illum quidem asperiores, cum nisi aperiam eius ipsa sapiente odit!</p>
            <button class="button btn">Start Looking</button>
        </div>
        <div class="image" >
        <img  width="100%" src="~assets/svg/fire-extinguisher.svg" alt="fire extinguisher">
        </div>

    </div>
</template>

<script>
    export default {}
</script>

<style scoped>
    .Hero {
        height: max-content;
        position: relative;
        display: flex;
        padding: 5rem 0;
        align-items: flex-start;
        justify-content: space-between;
    }
    .text-container {
        width: 50%;
        margin-top: 4rem;
    }
    .header {
        font-weight: 900;
        font-size: 5rem;
    }
    .snippet {
        color: grey;
        font-size: 1.25rem;
    }
    .image {
        width: 440px;
        height: 440px;
        margin-top: 2rem;
    }
    .button {
        padding: 1rem 4rem;
        border-radius: 100rem;
        color: rgb(231, 81, 43);
        background: white;
        border: 2px solid rgb(231, 81, 43);
        width: 20rem;
        font-weight: 700;
        transition: 0.2s;
        outline: none !important;
    }
    .button:hover {
        transform: scale(1.045);
        background: rgb(231, 81, 43);
        color: white;
    }
</style>