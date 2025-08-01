<template>
    <header class="grid-container w-full bg-white py-2.5 md:py-3.5 relative">
        <div class="flex items-center justify-between">
            <div class="flex items-center md:gap-24 lg:gap-14">
                <a href="/">
                    <img src="/images/header/logo.png" alt="" class="w-[132px] md:w-[157px]">
                </a>
                <div class="flex items-center md:gap-6 max-md:justify-between max-md:absolute max-md:w-full max-md:left-0 max-md:px-5 transition-all duration-500 max-md:top-full" :class="isMenuShow ? '' : 'max-md:-translate-x-full'">
                    <a href="#"
                        class="bg-[#EFEFEF] rounded-full py-[7px] px-4 text-sm font-medium leading-[100%]">Сервера</a>
                    <a href="#"
                        class="bg-[#F7F7F7] text-[#ADADAD] rounded-full py-[7px] px-4 text-sm font-medium leading-[100%] relative">
                        Счета
                        <span
                            class="absolute -top-px -right-px w-[13px] h-[13px] text-[8px] leading-[100%] font-semibold rounded-full bg-[#136BFB] text-white flex items-center justify-center">1</span>
                    </a>
                    <a href="#"
                        class="bg-[#136BFB] text-white rounded-full py-[7px] px-4 text-sm font-medium leading-[100%]">Заказать</a>
                </div>
            </div>
            <div class="flex items-center">
                <div class="flex items-center md:gap-3 max-md:rounded-full max-md:bg-[#F7F7F7] relative">
                    <div class="w-10 h-10 flex items-center justify-center bg-[#EFEFEF] rounded-full">
                        <img src="/images/header/avatar.png" alt="">
                    </div>
                    <button @click="isDropdownShow = !isDropdownShow"
                        class="cursor-pointer flex items-center gap-3 md:bg-[#F7F7F7] rounded-full max-md:h-full md:py-2.5 pl-1 md:pl-5 pr-4">
                        <span class="text-sm leading-[100%] font-medium max-md:hidden">Евгений Фадеев</span>
                        <img src="/images/header/arrow.png" alt="">
                    </button>
                    <!-- dropdown -->
                    <div v-show="isDropdownShow"
                        class="bg-white py-3 px-8 rounded-[20px] shadow-[0px_1px_22px_-1px_#00000014] text-sm leading-[29px] flex flex-col absolute right-0 top-[115%]">
                        <a href="#">Профиль</a>
                        <a href="#">Выйти</a>
                    </div>
                </div>
                <button @click="isMenuShow = !isMenuShow" class="ml-6 md:hidden flex flex-col justify-center items-center relative transition-all duration-300 ease-in-out w-7 h-5 cursour-pointer">
                    <span
                        class="absolute h-0.5 bg-[#ADADAD] rounded-[1px] transition-all duration-300 ease-in-out origin-center"
                        :class="isMenuShow ? 'w-[17px] rotate-45 translate-y-0' : 'w-7 -translate-y-1.5'"></span>
                    <span class="absolute h-0.5 bg-[#ADADAD] rounded-[1px] transition-all duration-300 ease-in-out"
                        :class="isMenuShow ? 'w-[17px] opacity-0 scale-0' : 'w-7 opacity-100 scale-100'"></span>
                    <span
                        class="absolute h-0.5 bg-[#ADADAD] rounded-[1px] transition-all duration-300 ease-in-out origin-center"
                        :class="isMenuShow ? 'w-[17px] -rotate-45 translate-y-0' : 'w-7 translate-y-1.5'"></span>
                </button>
            </div>
        </div>
    </header>
</template>

<script setup>
/* dropdown */
const isDropdownShow = ref(false)


/* menu */
const isMenuShow = ref(false)
</script>