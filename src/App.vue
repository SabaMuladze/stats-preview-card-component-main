
<template>
    <div class="min-h-screen w-full bg-[#0A0C1C] flex flex-col max-md:py-20 max-md:px-6">
        <div class="max-md:w-full bg-[#1B1937] rounded-lg">
            <div class="z-20 opacity-75 image relative">
                <img class="rounded-lg" src="src/assets/image-header-mobile.jpg" alt="">
            </div>
            <div class="px-6 mt-6 flex flex-col gap-6 text-center ">
                <h1 class="text-2xl">Get <span class="text-[#AB5CDB]">insights</span> that help your business
                    grow.
                </h1>
                <p class="opacity-75">Discover the benefits of data analytics and make better decisions regarding revenue,
                    customer
                    experience,
                    and overall efficiency.</p>
            </div>
            <div class="flex flex-col items-center mt-10 mb-8 gap-6">
                <div class="text-center">
                    <h2 class="text-2xl font-bold">{{ companies }}</h2>
                    <p class=" text-sm opacity-75">COMPANIES</p>
                </div>
                <div class="text-center">
                    <h2 class="text-2xl font-bold">{{ templates }}</h2>
                    <p class=" text-sm opacity-75">TEMPLATES</p>
                </div>
                <div class="text-center">

                    <h2 class="text-2xl font-bold">{{ queries }}</h2>
                    <p class=" text-sm opacity-75">QUERIES</p>
                </div>


            </div>
        </div>
    </div>
</template>

<script >
export default {
    data() {
        return {
            companies: '10K',
            templates: 314,
            queries: '12M+'
        }
    },
}
</script>

<style scoped>
h1 {
    font-weight: 700;
}

p {
    font-weight: 400;
}

.image::before {
    content: '';
    height: 100%;
    opacity: 70%;
    border-radius: 8px;
    mix-blend-mode: multiply;
    width: 100%;
    background-color: #AB5CDB;
    display: block;
    position: absolute;
    left: 0;
    top: 0;
    z-index: 100;
}
</style>
