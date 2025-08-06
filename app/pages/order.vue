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
        </div>
    </section>
</template>

<script setup>
</script>