<template>
    <section class="pt-9 grid-container bg-white">
        <div class="flex flex-col gap-1">
            <div class="flex items-center gap-4">
                <p class="text-[32px] leading-[100%] font-medium">Здравствуйте, Евгений!</p>
                <img src="/images/index/hand.png" alt="">
            </div>
            <div class="flex md:items-center md:justify-between max-md:flex-col max-md:gap-4">
                <p class="text-base leading-[100%] text-[#ADADAD]">Давайте посмотрим ваши данные по серверам</p>
                <label class="flex items-center gap-3 py-2 px-3.5 cursor-pointer group bg-[#F7F7F7] rounded-full w-fit">
                    <input type="checkbox" class="sr-only">
                    <span class="w-[18px] h-[18px] rounded-[3px] bg-[#EFEFEF] border border-[#E5E5E5] flex items-center justify-center transition-all duration-500 [.group:has(input:checked)_&]:bg-[#136BFB] [.group:has(input:checked)_&]:border-[#136BFB]">
                        <img src="/images/index/check.png" alt="" class="transition-all duration-500 opacity-0 group-hover:opacity-100 [.group:has(input:checked)_&]:opacity-100">
                    </span>
                    <span class="text-xs leading-[100%]">Показать только активные</span>
                </label>
            </div>
            <div class="flex items-center mt-8 md:mt-6 max-md:flex-col max-md:gap-1 max-md:pb-6">
                <div class="flex items-center justify-between py-2.5 md:py-4 px-4 md:px-5 w-full md:w-[244px] max-md:rounded-full md:rounded-t-[20px] max-md:bg-[#136BFB] max-md:text-white md:bg-[#F7F7F7] md:border border-[#F7F7F7]">
                    <div class="flex items-center gap-3.5 max-md:w-[65%] max-md:justify-between">
                        <span class="text-xl font-semibold leading-[100%] max-md:order-last">2</span>
                        <span class="text-base font-semibold leading-[100%]">Все сервера</span>
                    </div>
                    <div class="flex items-center gap-1">
                        <img src="/images/index/server_s.png" alt="">
                        <img src="/images/index/server_a.png" alt="">
                    </div>
                </div>
                <div class="flex items-center justify-between py-2.5 md:py-4 px-4 md:px-5 w-full md:w-[244px] max-md:rounded-full md:rounded-t-[20px] max-md:bg-[#F7F7F7] md:border border-[#EFEFEF]">
                    <div class="flex items-center gap-3.5 max-md:w-[65%] max-md:justify-between">
                        <span class="text-xl font-semibold leading-[100%] max-md:order-last">1</span>
                        <span class="text-base font-semibold leading-[100%]">Revit Server</span>
                    </div>
                    <img src="/images/index/server_s.png" alt="">
                </div>
                <div class="flex items-center justify-between py-2.5 md:py-4 px-4 md:px-5 w-full md:w-[244px] max-md:rounded-full md:rounded-t-[20px] max-md:bg-[#F7F7F7] md:border border-[#EFEFEF]">
                    <div class="flex items-center gap-3.5 max-md:w-[65%] max-md:justify-between">
                        <span class="text-xl font-semibold leading-[100%] max-md:order-last">1</span>
                        <span class="text-base font-semibold leading-[100%]">Revit Accelerator</span>
                    </div>
                    <img src="/images/index/server_a.png" alt="">
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>

</script>