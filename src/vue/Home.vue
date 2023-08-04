<script setup>
import Button from './../components/Button.vue'
import Title from './../components/Title.vue'
import Service from './../components/Service.vue'
import Why from './../components/Why.vue'
</script>

<template>
    <div>
    <section class="pt-16 pb-5">
        <div class="container flex flex-col gap-10">
            <div class="flex flex-col gap-8">
                <h1 class="text-purple text-4xl">IT Solutions that transform your business</h1>
                <div class="w-1/2">
                    <Button text="Learn more" />
                </div>
            </div>
            <div class="w-full">
                <img src="./../assets/img/home.webp" alt="Near By Site - Home" class="bg-cover">
            </div>
        </div>
    </section>

    <section class="py-24 bg-who bg-center bg-left w-full">
        <div class="container flex flex-col items-center justify-center gap-10 !py-10">
            <Title title="Who we are" />
            <p>Write a paragraph that talks about your company here. 
                You can talk about your company's background, history, mission,
                vision, or philosophy. Anything that will introduce your brand's
                persona to your clients. This will help build a connection between you and
                them, that hopefully leads into a working relationship.
            </p>
        </div>
    </section>

    <section class="py-10">
        <div class="container flex flex-col justify-center items-center gap-10">
            <Title title="Our Services" />
            <div>
                <Service />
            </div>
        </div>
    </section>

    <section class="py-10">
        <div class="container flex flex-col justify-center items-center gap-10">
            <Title title="Why choose us" />
            
            <Why />
           
        </div>
    </section>

   
</div>
</template>
