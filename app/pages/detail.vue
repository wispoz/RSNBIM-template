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
        </div>
    </section>
</template>

<script setup>

</script>