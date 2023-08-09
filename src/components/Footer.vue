<script setup>
import Button from './Button.vue'
import Title from './Title.vue'
</script>
<template>
    <footer>
        <div class="py-24 flex flex-col gap-10">
            <div class="container flex flex-col justify-center items-center gap-10">
                <div class="flex flex-col items-center gap-10">
                    <Title title="Contact Us" />
                    <!-- Formulaire de contact -->
                    <Button text="Send email" href="mailto:morgan.kpassi@gmail.com" />
                </div>
            </div>
        </div>
        <div class="container flex justify-between items-center gap-6 !py-5 bg-black text-sm">
            <p>Mentions legales</p>
            <p>Politique de confidentialité</p>
            <p>Copyright</p>
        </div>
    </footer>
</template>