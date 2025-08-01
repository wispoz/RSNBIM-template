<template>
    <header class="grid-container w-full bg-white py-2.5 md:py-3.5 relative">
        <div class="flex items-center justify-between">
            <div class="flex items-center md:gap-24 lg:gap-14">
                <a href="/">
                    <img src="/images/header/logo.png" alt="" class="w-[132px] md:w-[157px]">
                </a>
                <div class="flex items-center md:gap-6 max-md:justify-between max-md:absolute max-md:w-full max-md:top-full max-md:left-0">
                    <a href="#" class="bg-[#EFEFEF] rounded-full py-[7px] px-4 text-sm font-medium leading-[100%]">Сервера</a>
                    <a href="#" class="bg-[#F7F7F7] text-[#ADADAD] rounded-full py-[7px] px-4 text-sm font-medium leading-[100%] relative">
                        Счета
                        <span class="absolute -top-px -right-px w-[13px] h-[13px] text-[8px] leading-[100%] font-semibold rounded-full bg-[#136BFB] text-white flex items-center justify-center">1</span>
                    </a>
                    <a href="#" class="bg-[#136BFB] text-white rounded-full py-[7px] px-4 text-sm font-medium leading-[100%]">Заказать</a>
                </div>
            </div>
            <div class="flex items-center md:gap-3 max-md:rounded-full max-md:bg-[#F7F7F7]">
                <div class="w-10 h-10 flex items-center justify-center bg-[#EFEFEF] rounded-full">
                    <img src="/images/header/avatar.png" alt="">
                </div>
                <button class="flex items-center gap-3 md:bg-[#F7F7F7] rounded-full md:py-2.5 pl-1 md:pl-5 pr-4">
                    <span class="text-sm leading-[100%] font-medium max-md:hidden">Евгений Фадеев</span>
                    <img src="/images/header/arrow.png" alt="">
                </button>
            </div>
        </div>
    </header>
</template>

<script setup>

</script>