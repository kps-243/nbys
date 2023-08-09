<script setup>
import Button from './../components/Button.vue'
import Title from './../components/Title.vue'
import Service from './../components/Service.vue'
import Why from './../components/Why.vue'
import Project from './../components/Project.vue'
</script>

<template>
    <section class="pt-16 pb-5">
        <div class="container flex flex-col lg:flex-row lg:items-center gap-10">
            <div class="w-full lg:w-1/2 flex flex-col gap-8">
                <h1 class="text-purple text-4xl lg:text-7xl">IT Solutions that transform your business</h1>
                <div class="w-1/2">
                    <Button text="Learn more" />
                </div>
            </div>
            <div class="w-full lg:w-1/2">
                <img src="./../assets/img/home.webp" alt="Near By Site - Home" class="h-[700px] w-full">
            </div>
        </div>
    </section>

    <section class="py-24 bg-who bg-cover w-full">
        <div class="container mx-auto flex flex-col items-center justify-center gap-10 !py-10">
            <div class="flex flex-col gap-10 lg:px-24 text-center">
                <Title title="Who we are" />
                <p class="text-lg">Write a paragraph that talks about your company here. 
                    You can talk about your company's background, history, mission,
                    vision, or philosophy. Anything that will introduce your brand's
                    persona to your clients. This will help build a connection between you and
                    them, that hopefully leads into a working relationship.
                </p>
            </div>
        </div>
    </section>

    <section class="py-10">
        <div class="container flex flex-col justify-center items-center gap-10">
            <Title title="Our Services" />
            <Service />
        </div>
    </section>

    <section class="py-20">
        <div class="container flex flex-col justify-center items-center gap-10">
            <Title title="Why choose us" />
            <Why />
        </div>
    </section>
    
    <section class="py-24 bg-attention bg-center bg-cover w-full">
        <div class="container flex flex-col text-center gap-10 !py-10">
            <p class="lg:text-6xl">
                Grab the reader's attention with a descriptive line that hypes your event,
                product, or service. A short and relevant quote works, too!
            </p>
        </div>
    </section>
   
    <section class="py-10">
        <div class="container flex flex-col gap-12">
            <Title title="Projets" />
            <Project />
        </div>
    </section>
</template>
