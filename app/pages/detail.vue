<template>
    <section class="pt-9 grid-container bg-white">
        <div class="flex flex-col gap-4 md:gap-14 lg:gap-6">
            <div class="grid grid-cols-1 md:grid-cols-2 gap-3 md:gap-y-2.5 md:gap-x-5 lg:gap-4 lg:grid-cols-[45%_33%_22%]">
                <div class="flex items-center gap-2.5 lg:col-span-full">
                    <img src="/images/detail/arrow.png" alt="">
                    <p class="text-sm font-medium leading-[100%] text-[#ADADAD]">Все сервера</p>
                </div>
                <div class="flex flex-col gap-6 md:gap-4 text-white pt-1.5 md:pt-2.5 pb-5 px-4 md:px-5 rounded-[20px] bg-[#136BFB] relative md:order-3 lg:order-2">
                    <div class="flex flex-col gap-2 md:gap-3">
                        <p class="text-[28px] md:text-[32px] font-semibold leading-[100%]">Dev_serv</p>
                        <p class="text-sm font-medium leading-[100%]">Revit Server 2022</p>
                    </div>
                    <p class="text-[23px] md:text-[26px] font-semibold leading-[100%]">22 800 <span class="text-sm md:text-lg">₽/мес</span></p>
                    <img src="/images/index/server_s.png" alt="" class="absolute bottom-2 right-4 md:right-8 lg:right-5 w-[61px] md:w-[83px]">
                </div>
                <div class="flex flex-col gap-2 md:gap-6 pt-3 md:pt-4 pb-3.5 md:pb-4 lg:pb-5a px-5 rounded-[20px] [background:linear-gradient(90deg,#D8E4F9_0%,#EDF2FB_100%)] border-[0.5px] border-[#82A8EF] md:order-last lg:order-3">
                    <p class="text-lg md:text-[22px] font-semibold leading-[100%]">Тариф Pro-3</p>
                    <div class="flex flex-col gap-1 md:gap-0">
                        <div class="flex items-center gap-1 px-3 py-[3px] rounded-full bg-[#F0FEED] text-[#26C975] max-md:order-first w-fit">
                            <div class="w-1.5 h-1.5 rounded-full bg-[#26C975]"></div>
                            <p class="text-[13px] font-medium leading-[16px]">Активен</p>
                        </div>
                        <div class="flex max-md:flex-col md:items-center md:justify-between gap-3">
                            <p class="text-sm md:text-[13px] leading-[100%]">Оплачен до 15.03.2026</p>
                            <button class="py-2 w-40 text-center text-white bg-[#136BFB] rounded-[16px] text-sm font-semibold leading-[17px]">Продлить сервер</button>
                        </div>
                    </div>
                </div>
                <div class="flex lg:flex-col lg:gap-3 max-lg:items-center max-lg:justify-between py-2 lg:pt-2.5 lg:pb-5 px-4 lg:px-5 bg-[#F7F7F7] rounded-[20px] max-lg:h-fit md:order-2 lg:order-last">
                    <div class="flex lg:flex-col sm:gap-3 max-lg:items-center">
                        <img src="/images/detail/question.png" alt="" class="w-8 lg:w-10">
                        <p class="max-sm:hidden text-sm leading-[100%]">Помощь</p>
                    </div>
                    <button class="py-2 w-[173px] text-center bg-white text-[#136BFB] rounded-[16px] text-sm font-semibold leading-[17px]">Как подключиться</button>
                </div>
            </div>
            <div class="flex items-center max-md:flex-wrap gap-2.5 md:gap-1 max-md:text-[#ADADAD] text-sm font-medium leading-[100%] max-md:pb-7">
                <button @click="activeTab = 'tab1'" :class="{'!bg-[#136BFB] max-md:!text-white md:!bg-[#F7F7F7]' : activeTab === 'tab1'}" class="cursor-pointer transition-all duration-500 text-center max-md:rounded-full md:rounded-t-[20px] py-1.5 md:pt-2.5 md:pb-4 w-[134px] md:w-[150px] bg-[#F7F7F7] md:bg-white md:border border-[#EFEFEF]">Информация</button>
                <button @click="activeTab = 'tab2'" :class="{'!bg-[#136BFB] max-md:!text-white md:!bg-[#F7F7F7]' : activeTab === 'tab2'}" class="cursor-pointer transition-all duration-500 text-center max-md:rounded-full md:rounded-t-[20px] py-1.5 md:pt-2.5 md:pb-4 w-[134px] md:w-[150px] bg-[#F7F7F7] md:bg-white md:border border-[#EFEFEF]">Доступ по IP</button>
                <button @click="activeTab = 'tab3'" :class="{'!bg-[#136BFB] max-md:!text-white md:!bg-[#F7F7F7]' : activeTab === 'tab3'}" class="cursor-pointer transition-all duration-500 text-center max-md:rounded-full md:rounded-t-[20px] py-1.5 md:pt-2.5 md:pb-4 w-[134px] md:w-[150px] bg-[#F7F7F7] md:bg-white md:border border-[#EFEFEF]">Доступ по VPN</button>
                <button @click="activeTab = 'tab4'" :class="{'!bg-[#136BFB] max-md:!text-white md:!bg-[#F7F7F7]' : activeTab === 'tab4'}" class="cursor-pointer transition-all duration-500 text-center max-md:rounded-full md:rounded-t-[20px] py-1.5 md:pt-2.5 md:pb-4 w-[134px] md:w-[150px] bg-[#F7F7F7] md:bg-white md:border border-[#EFEFEF]">Логи сервера</button>
                <button @click="activeTab = 'tab5'" :class="{'!bg-[#136BFB] max-md:!text-white md:!bg-[#F7F7F7]' : activeTab === 'tab5'}" class="cursor-pointer transition-all duration-500 text-center max-md:rounded-full md:rounded-t-[20px] py-1.5 md:pt-2.5 md:pb-4 w-[134px] md:w-[150px] bg-[#F7F7F7] md:bg-white md:border border-[#EFEFEF]">Учет времени</button>
            </div>
        </div>
    </section>
    <section class="pt-6 md:pt-8 pb-11 grid-container">
        <TabsTab1 v-show="activeTab === 'tab1'"></TabsTab1>
        <TabsTab2 v-show="activeTab === 'tab2'"></TabsTab2>
        <TabsTab3 v-show="activeTab === 'tab3'"></TabsTab3>
        <TabsTab4 v-show="activeTab === 'tab4'"></TabsTab4>
    </section>
</template>

<script setup>
/* код табов */
const activeTab = ref('tab1')
</script>