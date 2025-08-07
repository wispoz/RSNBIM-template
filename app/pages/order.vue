<template>
    <section class="pt-9 pb-3.5 md:pb-6 grid-container bg-white">
        <p class="text-[28px] md:text-[32px] font-semibold leading-[100%]">Заказ сервера</p>
    </section>
    <section class="pt-6 md:pt-8 pb-11 grid-container">
        <div class="flex flex-col gap-5 max-md:col-span-full">
            <div class="w-full bg-white py-2.5 md:py-3.5 lg:py-4 px-6 lg:px-7 flex max-lg:flex-col gap-5 md:gap-8 lg:gap-[70px] rounded-[15px]">
                <div class="flex flex-col gap-5">
                    <div class="flex flex-col gap-6 md:gap-4 lg:gap-2.5">
                        <div class="flex items-center gap-5">
                            <img src="/images/detail/icon1.svg" alt="">
                            <p class="text-[22px] font-semibold leading-[100%]">Сервер</p>
                        </div>
                        <div class="flex flex-col gap-2.5">
                            <p class="text-sm font-semibold leading-[100%]">Название сервера</p>
                            <input value="jubilant-fertilizer" type="text" class="w-full text-xs px-4 py-2 leading-[100%] rounded-full border-[0.4px] border-[#ADADAD]">
                        </div>
                    </div>
                    <div class="flex flex-col gap-2.5">
                        <p class="text-sm font-semibold leading-[100%]">Роль сервера</p>
                        <div class="flex items-center max-sm:flex-col gap-4">
                            <label class="relative py-4 px-4 sm:px-5 h-[73px] sm:h-[103px] w-full sm:w-[275px] rounded-[20px] order-input">
                                <p class="text-base font-semibold leading-[100%]">Revit Server</p>
                                <img src="/images/index/server_s.png" alt="" class="absolute w-12 sm:w-[60px] top-2 sm:top-3.5 right-5 sm:right-2">
                                <input type="radio" name="server" checked class="sr-only">
                            </label>
                            <label class="relative py-4 px-4 sm:px-5 h-[73px] sm:h-[103px] w-full sm:w-[275px] rounded-[20px] order-input">
                                <p class="text-base font-semibold leading-[100%]">Revit Accelerator</p>
                                <img src="/images/index/server_a.png" alt="" class="absolute w-12 sm:w-[60px] top-2 sm:top-3.5 right-5 sm:right-2">
                                <input type="radio" name="server" class="sr-only">
                            </label>
                        </div>
                    </div>
                </div>
                <div class="flex flex-col gap-5">
                    <div class="flex flex-col gap-2.5">
                        <p class="text-sm font-semibold leading-[100%]">Версия сервера</p>
                        <div class="flex items-center gap-2.5 flex-wrap">
                            <label class="flex items-center justify-center w-16 md:w-[72px] h-6 md:h-7 rounded-full order-input">
                                <span>2019</span>
                                <input type="radio" name="year" checked class="sr-only">
                            </label>
                            <label class="flex items-center justify-center w-16 md:w-[72px] h-6 md:h-7 rounded-full order-input">
                                <span>2020</span>
                                <input type="radio" name="year" class="sr-only">
                            </label>
                            <label class="flex items-center justify-center w-16 md:w-[72px] h-6 md:h-7 rounded-full order-input">
                                <span>2021</span>
                                <input type="radio" name="year" class="sr-only">
                            </label>
                            <label class="flex items-center justify-center w-16 md:w-[72px] h-6 md:h-7 rounded-full order-input">
                                <span>2022</span>
                                <input type="radio" name="year" class="sr-only">
                            </label>
                            <label class="flex items-center justify-center w-16 md:w-[72px] h-6 md:h-7 rounded-full order-input">
                                <span>2023</span>
                                <input type="radio" name="year" class="sr-only">
                            </label>
                        </div>
                    </div>
                    <div class="flex flex-col gap-2.5">
                        <p class="text-sm font-semibold leading-[100%]">Локация</p>
                        <div class="flex items-center flex-wrap gap-3 md:gap-2 text-xs font-medium leading-[100%]">
                            <label class="py-1 px-2.5 md:px-3 order-input rounded-full flex items-center gap-1">
                                <img src="/images/order/ru.png" alt="">
                                <span>Москва</span>
                                <input type="radio" name="country" checked class="sr-only">
                            </label>
                            <label class="py-1 px-2.5 md:px-3 order-input rounded-full flex items-center gap-1">
                                <img src="/images/order/ru.png" alt="">
                                <span>Кемерево</span>
                                <input type="radio" name="country" class="sr-only">
                            </label>
                            <label class="py-1 px-2.5 md:px-3 order-input rounded-full flex items-center gap-1">
                                <img src="/images/order/ru.png" alt="">
                                <span>Саратов</span>
                                <input type="radio" name="country" class="sr-only">
                            </label>
                            <label class="py-1 px-2.5 md:px-3 order-input rounded-full flex items-center gap-1">
                                <img src="/images/order/ru.png" alt="">
                                <span>Владивосток</span>
                                <input type="radio" name="country" class="sr-only">
                            </label>
                            <label class="py-1 px-2.5 md:px-3 order-input rounded-full flex items-center gap-1">
                                <img src="/images/order/ru.png" alt="">
                                <span>Санкт-Петербург</span>
                                <input type="radio" name="country" class="sr-only">
                            </label>
                            <label class="py-1 px-2.5 md:px-3 order-input rounded-full flex items-center gap-1">
                                <img src="/images/order/ru.png" alt="">
                                <span>Казань</span>
                                <input type="radio" name="country" class="sr-only">
                            </label>
                            <label class="py-1 px-2.5 md:px-3 order-input rounded-full flex items-center gap-1">
                                <img src="/images/order/uae.png" alt="">
                                <span>ОАЭ</span>
                                <input type="radio" name="country" class="sr-only">
                            </label>
                            <label class="py-1 px-2.5 md:px-3 order-input rounded-full flex items-center gap-1">
                                <img src="/images/order/pl.png" alt="">
                                <span>Польша</span>
                                <input type="radio" name="country" class="sr-only">
                            </label>
                            <label class="py-1 px-2.5 md:px-3 order-input rounded-full flex items-center gap-1">
                                <img src="/images/order/de.png" alt="">
                                <span>Германия</span>
                                <input type="radio" name="country" class="sr-only">
                            </label>
                            <label class="py-1 px-2.5 md:px-3 order-input rounded-full flex items-center gap-1">
                                <img src="/images/order/nl.png" alt="">
                                <span>Амстердам</span>
                                <input type="radio" name="country" class="sr-only">
                            </label>
                            <label class="py-1 px-2.5 md:px-3 order-input rounded-full flex items-center gap-1">
                                <img src="/images/order/lv.png" alt="">
                                <span>Латвия</span>
                                <input type="radio" name="country" class="sr-only">
                            </label>
                        </div>
                    </div>
                </div>
            </div>
            <div class="w-full bg-white py-2.5 md:py-3.5 lg:py-4 px-6 lg:px-7 flex flex-col gap-5 md:gap-10 rounded-[15px]">
                <div class="flex flex-col gap-2 md:gap-4">
                    <div class="flex items-center gap-3 md:gap-5">
                        <img src="/images/order/icon.svg" alt="">
                        <p class="text-[22px] font-semibold leading-[100%]">Тариф</p>
                    </div>
                    <div class="grid grid-cols-2 md:grid-cols-3 xl:grid-cols-5 gap-x-3 gap-y-2 md:gap-4">
                        <label class="cursor-pointer group py-3 px-5 md:py-2 md:px-3 rounded-[20px] flex flex-col gap-2 md:gap-3.5 transition-all duration-500 [&:has(input:checked)]:bg-[#136BFB] [&:has(input:checked)]:border-[#136BFB] [&:has(input:checked)]:text-white bg-[#F7F7F7] border-[0.4px] border-[#ADADAD] ">
                            <input type="radio" name="rate" checked class="sr-only peer">
                            <div class="flex max-md:flex-col md:items-center gap-px justify-between">
                                <p class="text-xl md:text-[22px] font-semibold leading-[100%]">Start-2</p>
                                <img src="/images/order/1.svg" alt="" class="max-md:order-first w-8 md:w-10">
                            </div>
                            <div class="grid grid-cols-2 gap-x-1 gap-y-2 text-xs md:text-sm leading-[100%] w-fit text-[#ADADAD] transition-all duration-500 peer-checked:text-white">
                                <p class="font-semibold">4</p>
                                <p>CPU Core</p>
                                <p class="font-semibold">4 GB</p>
                                <p>RAM</p>
                                <p class="font-semibold">10 GB</p>
                                <p>NVME</p>
                                <p class="font-semibold">2-3</p>
                                <p>User</p>
                            </div>
                            <p class="text-lg md:text-2xl font-semibold leading-[100%]">7 900 <span class="text-base">₽/мес</span></p>
                        </label>
                        <label class="cursor-pointer group py-3 px-5 md:py-2 md:px-3 rounded-[20px] flex flex-col gap-2 md:gap-3.5 transition-all duration-500 [&:has(input:checked)]:bg-[#136BFB] [&:has(input:checked)]:border-[#136BFB] [&:has(input:checked)]:text-white bg-[#F7F7F7] border-[0.4px] border-[#ADADAD] ">
                            <input type="radio" name="rate" class="sr-only peer">
                            <div class="flex max-md:flex-col md:items-center gap-px justify-between">
                                <p class="text-xl md:text-[22px] font-semibold leading-[100%]">Start-3</p>
                                <img src="/images/order/2.svg" alt="" class="max-md:order-first w-8 md:w-10">
                            </div>
                            <div class="grid grid-cols-2 gap-x-1 gap-y-2 text-xs md:text-sm leading-[100%] w-fit text-[#ADADAD] transition-all duration-500 peer-checked:text-white">
                                <p class="font-semibold">6</p>
                                <p>CPU Core</p>
                                <p class="font-semibold">12 GB</p>
                                <p>RAM</p>
                                <p class="font-semibold">10 GB</p>
                                <p>NVME</p>
                                <p class="font-semibold">2-3</p>
                                <p>User</p>
                            </div>
                            <p class="text-lg md:text-2xl font-semibold leading-[100%]">9 900 <span class="text-base">₽/мес</span></p>
                        </label>
                        <label class="cursor-pointer group py-3 px-5 md:py-2 md:px-3 rounded-[20px] flex flex-col gap-2 md:gap-3.5 transition-all duration-500 [&:has(input:checked)]:bg-[#136BFB] [&:has(input:checked)]:border-[#136BFB] [&:has(input:checked)]:text-white bg-[#F7F7F7] border-[0.4px] border-[#ADADAD] ">
                            <input type="radio" name="rate" class="sr-only peer">
                            <div class="flex max-md:flex-col md:items-center gap-px justify-between">
                                <p class="text-xl md:text-[22px] font-semibold leading-[100%]">Standart-3</p>
                                <img src="/images/order/3.svg" alt="" class="max-md:order-first w-8 md:w-10">
                            </div>
                            <div class="grid grid-cols-2 gap-x-1 gap-y-2 text-xs md:text-sm leading-[100%] w-fit text-[#ADADAD] transition-all duration-500 peer-checked:text-white">
                                <p class="font-semibold">8</p>
                                <p>CPU Core</p>
                                <p class="font-semibold">16 GB</p>
                                <p>RAM</p>
                                <p class="font-semibold">30 GB</p>
                                <p>NVME</p>
                                <p class="font-semibold">3-6</p>
                                <p>User</p>
                            </div>
                            <p class="text-lg md:text-2xl font-semibold leading-[100%]">11 900 <span class="text-base">₽/мес</span></p>
                        </label>
                        <label class="cursor-pointer group py-3 px-5 md:py-2 md:px-3 rounded-[20px] flex flex-col gap-2 md:gap-3.5 transition-all duration-500 [&:has(input:checked)]:bg-[#136BFB] [&:has(input:checked)]:border-[#136BFB] [&:has(input:checked)]:text-white bg-[#F7F7F7] border-[0.4px] border-[#ADADAD] ">
                            <input type="radio" name="rate" class="sr-only peer">
                            <div class="flex max-md:flex-col md:items-center gap-px justify-between">
                                <p class="text-xl md:text-[22px] font-semibold leading-[100%]">Pro-3</p>
                                <img src="/images/order/4.svg" alt="" class="max-md:order-first w-8 md:w-10">
                            </div>
                            <div class="grid grid-cols-2 gap-x-1 gap-y-2 text-xs md:text-sm leading-[100%] w-fit text-[#ADADAD] transition-all duration-500 peer-checked:text-white">
                                <p class="font-semibold">12</p>
                                <p>CPU Core</p>
                                <p class="font-semibold">24 GB</p>
                                <p>RAM</p>
                                <p class="font-semibold">60 GB</p>
                                <p>NVME</p>
                                <p class="font-semibold">8-12</p>
                                <p>User</p>
                            </div>
                            <p class="text-lg md:text-2xl font-semibold leading-[100%]">13 900 <span class="text-base">₽/мес</span></p>
                        </label>
                        <label class="cursor-pointer group py-3 px-5 md:py-2 md:px-3 rounded-[20px] flex flex-col gap-2 md:gap-3.5 transition-all duration-500 [&:has(input:checked)]:bg-[#136BFB] [&:has(input:checked)]:border-[#136BFB] [&:has(input:checked)]:text-white bg-[#F7F7F7] border-[0.4px] border-[#ADADAD] ">
                            <input type="radio" name="rate" class="sr-only peer">
                            <div class="flex max-md:flex-col md:items-center gap-px justify-between">
                                <p class="text-xl md:text-[22px] font-semibold leading-[100%]">Pro-4</p>
                                <img src="/images/order/5.svg" alt="" class="max-md:order-first w-8 md:w-10">
                            </div>
                            <div class="grid grid-cols-2 gap-x-1 gap-y-2 text-xs md:text-sm leading-[100%] w-fit text-[#ADADAD] transition-all duration-500 peer-checked:text-white">
                                <p class="font-semibold">16</p>
                                <p>CPU Core</p>
                                <p class="font-semibold">32 GB</p>
                                <p>RAM</p>
                                <p class="font-semibold">60 GB</p>
                                <p>NVME</p>
                                <p class="font-semibold">8-12</p>
                                <p>User</p>
                            </div>
                            <p class="text-lg md:text-2xl font-semibold leading-[100%]">15 900 <span class="text-base">₽/мес</span></p>
                        </label>
                    </div>
                </div>
                <div class="flex max-xl:flex-col gap-12 xl:justify-between">
                    <div class="flex flex-col gap-2.5">
                        <p class="text-sm font-semibold leading-[100%]">Период оплаты</p>
                        <div class="flex items-center flex-wrap gap-1.5 md:gap-4 text-xs font-semibold leading-[100%]">
                            <label class="order-input rounded-full flex items-center justify-center w-[73px] md:w-20 h-6 md:h-7">
                                <span>1 мес.</span>
                                <input type="radio" checked name="period" class="sr-only">
                            </label>
                            <label class="order-input rounded-full flex items-center justify-center w-[73px] md:w-20 h-6 md:h-7">
                                <span>3 мес.</span>
                                <input type="radio" name="period" class="sr-only">
                            </label>
                            <label class="order-input rounded-full flex items-center justify-center w-[73px] md:w-20 h-6 md:h-7">
                                <span>6 мес.</span>
                                <input type="radio" name="period" class="sr-only">
                            </label>
                            <label class="order-input rounded-full flex items-center justify-center w-[73px] md:w-20 h-6 md:h-7">
                                <span>12 мес.</span>
                                <input type="radio" name="period" class="sr-only">
                            </label>
                            <label class="order-input rounded-full flex items-center justify-center w-[73px] md:w-20 h-6 md:h-7">
                                <span>24 мес.</span>
                                <input type="radio" name="period" class="sr-only">
                            </label>
                        </div>
                    </div>
                    <div class="flex flex-col gap-2.5">
                        <p class="text-sm font-semibold leading-[100%]">Бэкап - резервное копирование</p>
                        <div class="flex md:items-center gap-1 md:gap-6">
                            <div class="group relative w-full md:w-[272px]">
                                <input type="radio" id="backup-14" name="backup" class="sr-only peer">
                                <label for="backup-14" class="cursor-pointer transition-all duration-500 w-full py-3 px-2.5 md:px-4 rounded-[15px] bg-[#F7F7F7] border border-[#EFEFEF] flex items-center justify-between peer-checked:[background:linear-gradient(90deg,#D8E4F9_0%,#EDF2FB_100%)] peer-checked:border-[#136BFB]">
                                    <div class="flex items-center gap-4">
                                        <p class="text-sm font-semibold leading-[100%]">14 дней</p>
                                        <p class="text-xs leading-[100%]">500 ₽</p>  
                                    </div>
                                    <div class="w-[34px] h-[15px] flex items-center bg-[#D9D9D9] px-px rounded-[15px] transition-all duration-500 [.group:has(input:checked)_&]:bg-[#136BFB]">
                                        <div class="w-[13px] h-[13px] bg-white rounded-full transition-all duration-500 [.group:has(input:checked)_&]:translate-x-[19px]"></div>
                                    </div>
                                </label>
                            </div>
                            <div class="group relative w-full md:w-[272px]">
                                <input type="radio" id="backup-30" name="backup" class="sr-only peer">
                                <label for="backup-30" class="cursor-pointer transition-all duration-500 w-full py-3 px-2.5 md:px-4 rounded-[15px] bg-[#F7F7F7] border border-[#EFEFEF] flex items-center justify-between peer-checked:[background:linear-gradient(90deg,#D8E4F9_0%,#EDF2FB_100%)] peer-checked:border-[#136BFB]">
                                    <div class="flex items-center gap-4">
                                        <p class="text-sm font-semibold leading-[100%]">30 дней</p>
                                        <p class="text-xs leading-[100%]">1 000 ₽</p>  
                                    </div>
                                    <div class="w-[34px] h-[15px] flex items-center bg-[#D9D9D9] px-px rounded-[15px] transition-all duration-500 [.group:has(input:checked)_&]:bg-[#136BFB]">
                                        <div class="w-[13px] h-[13px] bg-white rounded-full transition-all duration-500 [.group:has(input:checked)_&]:translate-x-[19px]"></div>
                                    </div>
                                </label>
                            </div>
                        </div>
                        <p class="text-xs leading-[100%] text-[#ADADAD]">Резервное копирование проектов за последние 14/30 дней</p>
                    </div>
                </div>
            </div>
        </div>
        <div class="mt-5 md:mt-9 flex max-md:flex-col items-center md:items-end w-fit lg:ml-auto gap-9 md:gap-[90px]">
            <div class="grid grid-cols-2 gap-x-6 gap-y-2 text-xs text-[#ADADAD] leading-[100%]">
                <p>Тариф Start-2</p>
                <p class="font-semibold">7 900 ₽ / мес</p>
                <p>Бэкап 30 дней</p>
                <p class="font-semibold">1 000 ₽ / мес</p>
                <p class="text-base font-semibold text-[#0F0F0F]">ИТОГО</p>
                <p class="text-base font-semibold text-[#0F0F0F]">8 900 ₽ / мес</p>
            </div>
            <button class="cursor-pointer w-[212px] h-[34px] flex items-center justify-center text-white bg-[#136BFB] text-sm font-semibold leading-[100%] rounded-full">Заказать</button>
        </div>
    </section>
</template>

<script setup>
</script>