
<template>
    <div class="min-h-screen w-full bg-[#0A0C1C] flex flex-col py-20 px-6 md:items-center md:justify-center ">
        <div class="max-md:w-full bg-[#1B1937] rounded-lg md:flex md:flex-row-reverse max-w-[1100px]">
            <div class="z-20 opacity-75 relative image md:w-[50%]">
                <img class="rounded-lg  md:hidden object-cover w-full" src="src/assets/image-header-mobile.jpg" alt="">
                <div class="max-sm:hidden img rounded-lg"></div>
            </div>
            <div class="md:flex-1 md:pt-16 md:px-14 mt-10">
                <div class="px-6 mt-6 flex flex-col gap-6 text-center md:text-left md:px-0 md:mt-0">
                    <h1 class="text-2xl md:text-4xl">Get <span class="text-[#AB5CDB]">insights</span> that help your
                        business
                        grow.
                    </h1>
                    <p class="opacity-75">Discover the benefits of data analytics and make better decisions regarding
                        revenue,
                        customer
                        experience,
                        and overall efficiency.</p>
                </div>
                <div
                    class="flex flex-col items-center mt-10 mb-8 gap-6 md:flex-row md:justify-between lg:pb-8 md:mt-[72px]">
                    <div class="text-center md:text-left">
                        <h2 class="text-2xl font-bold">{{ companies }}</h2>
                        <p class=" text-sm opacity-75">COMPANIES</p>
                    </div>
                    <div class="text-center md:text-left">
                        <h2 class="text-2xl font-bold">{{ templates }}</h2>
                        <p class=" text-sm opacity-75">TEMPLATES</p>
                    </div>
                    <div class="text-center md:text-left">
                        <h2 class="text-2xl font-bold">{{ queries }}</h2>
                        <p class=" text-sm opacity-75">QUERIES</p>
                    </div>
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
    border-radius: 5px;
    mix-blend-mode: multiply;
    width: 100%;
    background-color: #AB5CDB;
    display: block;
    position: absolute;
    left: 0;
    top: 0;
    z-index: 100;
}

.img {
    width: 100%;
    height: 100%;
    background-image: url('src/assets/image-header-desktop.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    object-fit: cover;
}
</style>
