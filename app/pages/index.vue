<template>
    <section class="pt-9 grid-container bg-white">
        <div class="flex flex-col gap-1">
            <div class="flex items-center gap-4">
                <p class="text-[32px] leading-[100%] font-medium">Здравствуйте, Евгений!</p>
                <img src="/images/index/hand.png" alt="">
            </div>
            <div class="flex md:items-center md:justify-between max-md:flex-col max-md:gap-4 max-md:mt-4">
                <p class="text-base leading-[100%] text-[#ADADAD]">Давайте посмотрим ваши данные по серверам</p>
                <label class="flex items-center gap-3 py-2 px-3.5 cursor-pointer group bg-[#F7F7F7] rounded-full w-fit max-md:hidden">
                    <input type="checkbox" class="sr-only">
                    <span class="w-[18px] h-[18px] rounded-[3px] bg-[#EFEFEF] border border-[#E5E5E5] flex items-center justify-center transition-all duration-500 [.group:has(input:checked)_&]:bg-[#136BFB] [.group:has(input:checked)_&]:border-[#136BFB]">
                        <img src="/images/index/check.png" alt="" class="transition-all duration-500 opacity-0 [.group:has(input:checked)_&]:opacity-100">
                    </span>
                    <span class="text-xs leading-[100%]">Показать только активные</span>
                </label>
            </div>
            <div class="flex items-center mt-8 md:mt-6 max-md:flex-col max-md:gap-1 max-md:pb-6">
                <label class="transition-all duration-500 cursor-pointer flex items-center justify-between py-2.5 md:py-4 px-4 md:px-5 w-full md:w-[244px] max-md:rounded-full md:rounded-t-[20px] max-md:bg-[#F7F7F7] md:border border-[#EFEFEF] max-md:[&:has(input:checked)]:bg-[#136BFB] max-md:[&:has(input:checked)]:text-white md:[&:has(input:checked)]:bg-[#F7F7F7] md:[&:has(input:checked)]:border-[#F7F7F7]">
                    <div class="flex items-center gap-3.5 max-md:w-[180px] max-md:justify-between">
                        <span class="text-xl font-semibold leading-[100%] max-md:order-last max-md:min-w-3">2</span>
                        <span class="text-base font-semibold leading-[100%]">Все сервера</span>
                    </div>
                    <div class="flex items-center gap-1">
                        <img src="/images/index/server_s.png" alt="" class="w-6">
                        <img src="/images/index/server_a.png" alt="" class="w-6">
                    </div>
                    <input type="radio" name="servers" class="sr-only" checked>
                </label>
                <label class="transition-all duration-500 cursor-pointer flex items-center justify-between py-2.5 md:py-4 px-4 md:px-5 w-full md:w-[244px] max-md:rounded-full md:rounded-t-[20px] max-md:bg-[#F7F7F7] md:border border-[#EFEFEF] max-md:[&:has(input:checked)]:bg-[#136BFB] max-md:[&:has(input:checked)]:text-white md:[&:has(input:checked)]:bg-[#F7F7F7] md:[&:has(input:checked)]:border-[#F7F7F7]">
                    <div class="flex items-center gap-3.5 max-md:w-[180px] max-md:justify-between">
                        <span class="text-xl font-semibold leading-[100%] max-md:order-last max-md:min-w-3">1</span>
                        <span class="text-base font-semibold leading-[100%]">Revit Server</span>
                    </div>
                    <img src="/images/index/server_s.png" alt="" class="w-6">
                    <input type="radio" name="servers" class="sr-only">
                </label>
                <label class="transition-all duration-500 cursor-pointer flex items-center justify-between py-2.5 md:py-4 px-4 md:px-5 w-full md:w-[244px] max-md:rounded-full md:rounded-t-[20px] max-md:bg-[#F7F7F7] md:border border-[#EFEFEF] max-md:[&:has(input:checked)]:bg-[#136BFB] max-md:[&:has(input:checked)]:text-white md:[&:has(input:checked)]:bg-[#F7F7F7] md:[&:has(input:checked)]:border-[#F7F7F7]">
                    <div class="flex items-center gap-3.5 max-md:w-[180px] max-md:justify-between">
                        <span class="text-xl font-semibold leading-[100%] max-md:order-last max-md:min-w-3">1</span>
                        <span class="text-base font-semibold leading-[100%]">Revit Accelerator</span>
                    </div>
                    <img src="/images/index/server_a.png" alt="" class="w-6">
                    <input type="radio" name="servers" class="sr-only">
                </label>
            </div>
        </div>
    </section>
    <section class="pt-6 md:pt-8 pb-11 grid-container">
        <label class="flex items-center gap-3 cursor-pointer group rounded-full w-fit md:hidden pb-3.5">
            <input type="checkbox" class="sr-only">
            <span class="w-[18px] h-[18px] rounded-[3px] bg-[#EFEFEF] border border-[#E5E5E5] flex items-center justify-center transition-all duration-500 [.group:has(input:checked)_&]:bg-[#136BFB] [.group:has(input:checked)_&]:border-[#136BFB]">
                <img src="/images/index/check.png" alt="" class="transition-all duration-500 opacity-0 [.group:has(input:checked)_&]:opacity-100">
            </span>
            <span class="text-xs leading-[100%]">Показать только активные</span>
        </label>
        <div class="grid grid-cols-1 md:grid-cols-2 xl:grid-cols-3 gap-4 lg:gap-x-5">
            <div class="rounded-[20px] pt-6 md:pt-4 pb-3 md:pb-5 px-4 md:px-6 bg-white relative">
                <div class="flex flex-col gap-2.5">
                    <div class="flex md:items-center md:justify-between gap-1.5 md:gap-4 max-md:flex-col">
                        <a href="/detail" class="truncate text-2xl font-semibold leading-[100%]">Dev_serv</a>
                        <div class="flex items-center gap-1 px-3 py-[3px] rounded-full bg-[#F0FEED] text-[#26C975] max-md:order-first w-fit shrink-0">
                            <div class="w-1.5 h-1.5 rounded-full bg-[#26C975]"></div>
                            <p class="text-[13px] font-medium leading-[100%]">Активен</p>
                        </div>
                    </div>
                    <p class="text-base font-medium leading-[100%]">Revit Server 2022</p>
                </div>
                <div class="grid grid-cols-2 gap-y-1 gap-x-5 text-xs leading-[100%] mt-5 w-fit">
                    <p>Создан</p>
                    <p>14.03.2025</p>
                    <p>Оплачен до</p>
                    <p>15.03.2026</p>
                    <p>Тариф</p>
                    <p>Pro-3</p>
                    <p>Локация</p>
                    <p>Москва</p>
                </div>
                <div class="flex max-md:flex-col max-md:gap-8 md:items-center md:justify-between mt-6 md:mt-7">
                    <a href="#" class="text-[#136BFB] text-[13px] font-medium leading-[100%]">saеvyсa9g0hq.rsnbim.ru</a>
                    <p class="font-semibold leading-[100%] text-2xl max-md:w-20">21 800 <span class="text-base">₽/мес</span></p>
                </div>
                <img src="/images/index/server_s.png" alt="" class="absolute right-4 md:right-8 bottom-3 md:bottom-[51px]">
            </div>
            <div class="rounded-[20px] pt-6 md:pt-4 pb-3 md:pb-5 px-4 md:px-6 bg-white relative">
                <div class="flex flex-col gap-2.5">
                    <div class="flex md:items-center md:justify-between gap-1.5 md:gap-4 max-md:flex-col">
                        <a href="/detail" class="truncate text-2xl font-semibold leading-[100%]">Dev_serv2223gdfgdfgdfdgfdgfgdf</a>
                        <div class="flex items-center gap-1 px-3 py-[3px] rounded-full bg-[#FDF1F2] text-[#FF6170] max-md:order-first w-fit shrink-0">
                            <div class="w-1.5 h-1.5 rounded-full bg-[#FF6170]"></div>
                            <p class="text-[13px] font-medium leading-[100%]">Ожидает оплаты</p>
                        </div>
                    </div>
                    <p class="text-base font-medium leading-[100%]">Revit Accelerator 2022</p>
                </div>
                <div class="grid grid-cols-2 gap-y-1 gap-x-5 text-xs leading-[100%] mt-5 w-fit">
                    <p>Создан</p>
                    <p>14.03.2025</p>
                    <p>Оплачен до</p>
                    <p>15.03.2026</p>
                    <p>Тариф</p>
                    <p>Pro-3</p>
                    <p>Локация</p>
                    <p>Москва</p>
                </div>
                <div class="flex max-md:flex-col max-md:gap-8 md:items-center md:justify-between mt-6 md:mt-7">
                    <a href="#" class="text-[#136BFB] text-[13px] font-medium leading-[100%]">saеvyсa9g0hq.rsnbim.ru</a>
                    <p class="font-semibold leading-[100%] text-2xl max-md:w-20">21 800 <span class="text-base">₽/мес</span></p>
                </div>
                <img src="/images/index/server_a.png" alt="" class="absolute right-4 md:right-8 bottom-3 md:bottom-[51px] opacity-50">
            </div>
            <div class="rounded-[20px] py-8 md:py-6 px-[18px] md:px-6 flex flex-col justify-between bg-[#136BFB] text-white gap-8 max-lg:order-first">
                <div class="flex flex-col gap-1">
                    <p class="text-[13px] font-medium leading-[100%]">ВСЕГО 3 УСЛУГИ НА СУММУ</p>
                    <p class="text-4xl font-semibold leading-[100%] max-md:max-w-[135px]">44 600 <span class="text-[22px]">₽/мес</span></p>
                </div>
                <div class="flex flex-col gap-2.5">
                    <p class="text-sm font-medium leading-[100%]">Ожидает оплаты</p>
                    <div class="relative max-md:flex flex-col max-md:flex-col max-md:gap-1.5">
                        <p class="w-full bg-[#2F81FE] pl-6 py-2 rounded-[24px] text-2xl font-semibold leading-[100%]">21 800 <span class="text-base">₽</span></p>
                        <a href="/accounts" class="px-4 py-3.5 md:py-2.5 rounded-[19px] w-fit bg-[#58A0FA] text-sm font-medium leading-[100%] md:absolute md:top-1/2 md:-translate-y-1/2 md:right-1 max-md:w-full max-md:text-center">Оплатить</a>
                    </div>
                </div>
            </div>
            <a href="/order" class="cursor-pointer rounded-[15px] border border-dashed border-[#136BFB] pt-3 pb-7 flex flex-col gap-1 items-center w-full text-center [background:linear-gradient(90deg,#D8E4F9_0%,#EDF2FB_100%)] h-fit">
                <img src="/images/index/plus.png" alt="">
                <span class="text-sm font-semibold leading-[100%]">Создать новый сервер</span>
            </a>
        </div>
    </section>
</template>

<script setup>

</script>