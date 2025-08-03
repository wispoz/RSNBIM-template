<template>
    <div class="flex flex-col">
        <div class="flex items-center max-md:flex-wrap gap-2.5 md:gap-1 max-md:text-[#ADADAD] text-sm font-medium leading-[100%] max-md:pb-7">
            <button @click="activeTab = 'tab1'" :class="{'!bg-[#136BFB] max-md:!text-white md:!bg-white md:!border-white' : activeTab === 'tab1'}" class="cursor-pointer transition-all duration-500 text-center max-md:rounded-full md:rounded-t-[20px] py-1.5 md:pt-2.5 md:pb-4 w-[134px] md:w-[139px] bg-white md:bg-transparent md:border border-[#E2E2E2]">Отчет</button>
            <button @click="activeTab = 'tab2'" :class="{'!bg-[#136BFB] max-md:!text-white md:!bg-white md:!border-white' : activeTab === 'tab2'}" class="cursor-pointer transition-all duration-500 text-center max-md:rounded-full md:rounded-t-[20px] py-1.5 md:pt-2.5 md:pb-4 w-[134px] md:w-[139px] bg-white md:bg-transparent md:border border-[#E2E2E2]">Пользователи</button>
        </div>
        <div class="rounded-[14px] md:rounded-tl-none bg-white max-md:mt-2.5 px-4 py-5 md:py-4 xl:px-6">
            <div v-show="activeTab === 'tab1'" class="flex flex-col gap-6 md:gap-8 w-full">
                <div class="flex flex-col gap-4">
                    <div class="flex items-center gap-3.5 py-1.5 px-5 rounded-full bg-[#F7F7F7] w-fit">
                        <label>
                            <input type="date" class="sr-only">
                            <img src="/images/detail/date.png" alt="">
                        </label>
                        <p class="text-sm leading-[100%]">10.07.2025 - 16.07.2025</p>
                    </div>
                </div>
                <div class="grid grid-cols-2 md:grid-cols-4 gap-1 md:gap-2">
                    <div class="flex flex-col gap-1 rounded-[10px] px-2 pt-1.5 pb-3.5 md:px-5 md:pt-2 md:pb-3 text-white bg-[#136BFB]">
                        <div class="flex items-center justify-between">
                            <p class="text-[20px] md:text-[30px] font-semibold leading-[100%]">100</p>
                            <img src="/images/detail/clock.png" alt="">
                        </div>
                        <p class="text-sm md:text-lg font-semibold leading-[100%]">Отработанное время</p>
                    </div>
                    <div class="flex flex-col gap-1 rounded-[10px] px-2 pt-1.5 pb-3.5 md:px-5 md:pt-2 md:pb-3 text-white bg-[#26C975]">
                        <div class="flex items-center justify-between">
                            <p class="text-[20px] md:text-[30px] font-semibold leading-[100%]">30</p>
                            <img src="/images/detail/add.png" alt="">
                        </div>
                        <p class="text-sm md:text-lg font-semibold leading-[100%]">Созданных элементов</p>
                    </div>
                    <div class="flex flex-col gap-1 rounded-[10px] px-2 pt-1.5 pb-3.5 md:px-5 md:pt-2 md:pb-3 text-white bg-[#EFB000]">
                        <div class="flex items-center justify-between">
                            <p class="text-[20px] md:text-[30px] font-semibold leading-[100%]">30</p>
                            <img src="/images/detail/edit2.png" alt="">
                        </div>
                        <p class="text-sm md:text-lg font-semibold leading-[100%]">Измененных элементов</p>
                    </div>
                    <div class="flex flex-col gap-1 rounded-[10px] px-2 pt-1.5 pb-3.5 md:px-5 md:pt-2 md:pb-3 text-white bg-[#FF6170]">
                        <div class="flex items-center justify-between">
                            <p class="text-[20px] md:text-[30px] font-semibold leading-[100%]">10</p>
                            <img src="/images/detail/delete2.png" alt="">
                        </div>
                        <p class="text-sm md:text-lg font-semibold leading-[100%]">Удаленных элементов</p>
                    </div>
                </div>

            </div>
        </div>
    </div>
</template>

<script setup>
/* код табов */
const activeTab = ref('tab1')
</script>