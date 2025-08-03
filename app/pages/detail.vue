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
    <section class="pt-6 md:pt-8 grid-container">
        <div class="grid grid-cols-1 md:grid-cols-2 xl:grid-cols-3 gap-3.5 md:gap-y-4 md:gap-x-5">
            <div class="bg-white rounded-[15px] py-3.5 md:pt-2 md:pb-5 px-4 md:px-5 flex flex-col gap-3 md:gap-5">
                <div class="flex items-center gap-2 md:gap-4">
                    <img src="/images/detail/icon1.svg" alt="">
                    <p class="text-base font-semibold leading-[100%]">О сервере</p>
                </div>
                <div class="grid grid-cols-2 text-xs leading-[100%] gap-x-1.5 md:gap-x-[59px] gap-y-3.5">
                    <p class="odd:text-[#ADADAD]">Название сервера</p>
                    <p class="odd:text-[#ADADAD]">Dev_serv</p>
                    <p class="odd:text-[#ADADAD]">Роль</p>
                    <p class="odd:text-[#ADADAD]">Revit Server</p>
                    <p class="odd:text-[#ADADAD]">Версия сервера</p>
                    <p class="odd:text-[#ADADAD]">Revit Server 2022</p>
                    <p class="odd:text-[#ADADAD]">Тариф</p>
                    <p class="odd:text-[#ADADAD]">Pro-3</p>
                    <p class="odd:text-[#ADADAD]">Дата создания</p>
                    <p class="odd:text-[#ADADAD]">14.03.2025</p>
                    <p class="odd:text-[#ADADAD]">Активен до</p>
                    <p class="odd:text-[#ADADAD]">15.03.2026</p>
                    <p class="odd:text-[#ADADAD]">Локация</p>
                    <p class="odd:text-[#ADADAD]">Москва</p>
                    <p class="odd:text-[#ADADAD]">Домен</p>
                    <p class="odd:text-[#ADADAD]"><a href="www.website.ru" target="_blank" class="text-[#136BFB]">www.website.ru</a></p>
                </div>
            </div>
            <div class="bg-white rounded-[15px] py-3.5 md:pt-2 md:pb-5 px-4 md:px-5 flex flex-col gap-3 md:gap-5">
                <div class="flex justify-between gap-3.5">
                    <div class="flex gap-2 md:gap-4">
                        <img src="/images/detail/icon2.svg" alt="" class="h-fit">
                        <div class="flex flex-col gap-1.5 mt-1.5">
                            <p class="text-base font-semibold leading-[100%]">Административная панель</p>
                            <p class="text-xs leading-[100%]">Revit Server</p>
                        </div>
                    </div>
                    <button class="cursor-pointer max-md:mt-auto">
                        <img src="/images/detail/eye.png" alt="" class="h-fit shrink-0">
                    </button>
                </div>
                <div class="grid grid-cols-2 gap-x-6 gap-y-3.5 md:gap-x-14 w-full text-xs leading-[100%]">
                    <p class="odd:text-[#ADADAD]">Revit Server <br> Administrator</p>
                    <button class="py-1 font-semibold text-[#136BFB] text-center border border-[#136BFB] w-[83px] rounded-full">Открыть</button>
                    <p class="odd:text-[#ADADAD]">Логин</p>
                    <div class="flex items-end justify-between grow">
                        <p>Login2333</p>
                        <button class="cursor-pointer">
                            <img src="/images/detail/copy.png" alt="">
                        </button>
                    </div>
                    <p class="odd:text-[#ADADAD]">Пароль</p>
                    <div class="flex items-end justify-between grow">
                        <p>q32eqq4qqq4q</p>
                        <button class="cursor-pointer">
                            <img src="/images/detail/copy.png" alt="">
                        </button>
                    </div>
                </div>
            </div>
            <div class="bg-white rounded-[15px] py-3.5 md:pt-2 md:pb-5 px-4 md:px-5 flex flex-col gap-3 md:gap-5">
                <div class="flex justify-between gap-3.5">
                    <div class="flex gap-2 md:gap-4">
                        <img src="/images/detail/icon3.svg" alt="" class="h-fit">
                        <div class="flex flex-col gap-1.5 mt-1.5">
                            <p class="text-base font-semibold leading-[100%]">Общие файлы на сервере</p>
                        </div>
                    </div>
                    <button class="cursor-pointer max-md:mt-auto">
                        <img src="/images/detail/eye.png" alt="" class="h-fit shrink-0">
                    </button>
                </div>
                <div class="grid grid-cols-2 gap-x-6 gap-y-3.5 md:gap-x-12 w-full text-xs leading-[100%]">
                    <p class="odd:text-[#ADADAD] max-md:col-span-full">Ссылка для проводника Windows</p>
                    <p class="odd:text-[#ADADAD] max-md:col-span-full">\\ it18kg9ewit4.rsnbim.ru \Share</p>
                    <p class="odd:text-[#ADADAD]">Логин</p>
                    <div class="flex items-end justify-between grow">
                        <div class="flex items-center gap-2">
                            <div class="w-1 h-1 rounded-full bg-black"></div>
                            <div class="w-1 h-1 rounded-full bg-black"></div>
                            <div class="w-1 h-1 rounded-full bg-black"></div>
                            <div class="w-1 h-1 rounded-full bg-black"></div>
                            <div class="w-1 h-1 rounded-full bg-black"></div>
                            <div class="w-1 h-1 rounded-full bg-black"></div>
                        </div>
                        <button class="cursor-pointer">
                            <img src="/images/detail/copy.png" alt="">
                        </button>
                    </div>
                    <p class="odd:text-[#ADADAD]">Пароль</p>
                    <div class="flex items-end justify-between grow">
                        <div class="flex items-center gap-2">
                            <div class="w-1 h-1 rounded-full bg-black"></div>
                            <div class="w-1 h-1 rounded-full bg-black"></div>
                            <div class="w-1 h-1 rounded-full bg-black"></div>
                            <div class="w-1 h-1 rounded-full bg-black"></div>
                            <div class="w-1 h-1 rounded-full bg-black"></div>
                            <div class="w-1 h-1 rounded-full bg-black"></div>
                        </div>
                        <button class="cursor-pointer">
                            <img src="/images/detail/copy.png" alt="">
                        </button>
                    </div>
                </div>
            </div>
            <div class="bg-white rounded-[15px] py-3.5 md:pt-2 md:pb-5 px-4 md:px-5 flex flex-col gap-3 md:gap-5">
                <div class="flex justify-between gap-3.5">
                    <div class="flex gap-2 md:gap-4">
                        <img src="/images/detail/icon3.svg" alt="" class="h-fit">
                        <div class="flex flex-col gap-1.5 mt-1.5">
                            <p class="text-base font-semibold leading-[100%]">Технические характеристики</p>
                        </div>
                    </div>
                </div>
                <div class="grid grid-cols-2 gap-y-3.5 gap-x-5 md:gap-x-[103px] text-xs leading-[100%]">
                    <p class="odd:text-[#ADADAD]">CPU</p>
                    <p class="odd:text-[#ADADAD]">12 cores</p>
                    <p class="odd:text-[#ADADAD]">RAM</p>
                    <p class="odd:text-[#ADADAD]">24 Gb</p>
                    <p class="odd:text-[#ADADAD]">SSD</p>
                    <p class="odd:text-[#ADADAD]">60 Gb</p>
                </div>
                <div class="w-full h-[0.25px] bg-[#ADADAD]"></div>
                <div class="flex flex-col gap-2.5">
                    <p class="text-sm font-semibold leading-[100%]">Бэкап - резервное копирование</p>
                    <div class="flex items-center gap-2 md:gap-3">
                        <div class="group relative w-1/2">
                            <input type="radio" id="backup-14" name="backup" class="sr-only peer">
                            <label for="backup-14" class="cursor-pointer transition-all duration-500 w-full py-2 md:pb-6 px-2.5 md:px-4 rounded-[15px] bg-[#F7F7F7] border border-[#EFEFEF] flex flex-col gap-1.5 md:gap-1.5 peer-checked:[background:linear-gradient(90deg,#D8E4F9_0%,#EDF2FB_100%)] peer-checked:border-[#136BFB]">
                                <div class="flex items-center justify-between gap-px">
                                    <p class="text-sm font-semibold leading-[100%]">14 дней</p>
                                    <div class="w-[34px] h-[15px] flex items-center bg-[#D9D9D9] px-px rounded-[15px] transition-all duration-500 [.group:has(input:checked)_&]:bg-[#136BFB]">
                                        <div class="w-[13px] h-[13px] bg-white rounded-full transition-all duration-500 [.group:has(input:checked)_&]:translate-x-[19px]"></div>
                                    </div>
                                </div>
                                <p class="text-xs leading-[100%]">500 ₽</p>  
                            </label>
                        </div>
                        <div class="group relative w-1/2">
                            <input type="radio" id="backup-30" name="backup" class="sr-only peer">
                            <label for="backup-30" class="cursor-pointer transition-all duration-500 w-full py-2 md:pb-6 px-2.5 md:px-4 rounded-[15px] bg-[#F7F7F7] border border-[#EFEFEF] flex flex-col gap-1.5 md:gap-1.5 peer-checked:[background:linear-gradient(90deg,#D8E4F9_0%,#EDF2FB_100%)] peer-checked:border-[#136BFB]">
                                <div class="flex items-center justify-between gap-px">
                                    <p class="text-sm font-semibold leading-[100%]">30 дней</p>
                                    <div class="w-[34px] h-[15px] flex items-center bg-[#D9D9D9] px-px rounded-[15px] transition-all duration-500 [.group:has(input:checked)_&]:bg-[#136BFB]">
                                        <div class="w-[13px] h-[13px] bg-white rounded-full transition-all duration-500 [.group:has(input:checked)_&]:translate-x-[19px]"></div>
                                    </div>
                                </div>
                                <p class="text-xs leading-[100%]">1 000 ₽</p>  
                            </label>
                        </div>
                    </div>
                    <p class="text-[13px] leading-[100%] text-[#ADADAD]">Резервное копирование проектов за последние 14/30 дней</p>
                </div>
            </div>
            <div class="bg-white rounded-[15px] py-3.5 md:pt-2 md:pb-5 px-4 md:px-5 flex flex-col gap-3 md:gap-5 md:col-span-2">
                <div class="flex justify-between gap-3.5">
                    <div class="flex gap-2 md:gap-4">
                        <img src="/images/detail/icon3.svg" alt="" class="h-fit">
                        <div class="flex flex-col gap-1.5 mt-1.5">
                            <p class="text-base font-semibold leading-[100%]">Объем места</p>
                        </div>
                    </div>
                </div>
                <div class="flex max-md:flex-col max-md:items-center gap-8 md:gap-28">
                    <div class="relative w-[238px] h-[238px] md:w-[253px] md:h-[253px]">
                        <svg class="w-full h-full transform -rotate-90" viewBox="0 0 255 255" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <!-- Фоновая окружность -->
                            <circle
                                cx="127.5"
                                cy="127.5"
                                r="106"
                                fill="none"
                                stroke="#EFEFEF"
                                stroke-width="43"
                            />
                            <!-- Заполненная часть (динамическая) -->
                            <circle
                                cx="127.5"
                                cy="127.5"
                                r="106"
                                fill="none"
                                stroke="#136BFB"
                                stroke-width="43"
                                stroke-linecap="round"
                                :stroke-dasharray="circumference"
                                :stroke-dashoffset="strokeDashoffset"
                                class="transition-all duration-500"
                            />
                        </svg>
                        <div class="absolute inset-0 flex flex-col gap-1 items-center justify-center">
                            <p class="text-[27px] font-semibold leading-[100%]">{{ totalSSD }}ГБ</p>
                            <p class="text-xs leading-[100%]">Объем SSD</p>
                        </div>
                    </div>
                    <div class="flex md:flex-col gap-5 md:gap-7">
                        <div class="flex items-start gap-2 md:gap-5">
                            <div class="w-4 h-4 bg-[#136BFB] rounded-full"></div>
                            <div class="flex flex-col gap-2 md:gap-2.5">
                                <p class="text-[22px] font-semibold leading-[100%]">{{ ssdUsage }}%</p>
                                <p class="text-xs leading-[100%]">Занято {{ usedSSD }} Гб</p>
                            </div>
                        </div>
                        <div class="flex items-start gap-2 md:gap-5">
                            <div class="w-4 h-4 bg-[#ADADAD] rounded-full"></div>
                            <div class="flex flex-col gap-2 md:gap-2.5">
                                <p class="text-[22px] font-semibold leading-[100%]">{{ 100 - ssdUsage }}%</p>
                                <p class="text-xs leading-[100%]">Свободно {{ freeSSD }} Гб</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>t
</template>

<script setup>
/* данные из БД */
const totalSSD = ref(60) // общий объем SSD в ГБ
const usedSSD = ref(30)  // использованный объем в ГБ

/* вычисляемые свойства */
const ssdUsage = computed(() => {
    return Math.round((usedSSD.value / totalSSD.value) * 100)
})

const freeSSD = computed(() => {
    return totalSSD.value - usedSSD.value
})

/* константы для SVG */
const radius = 106
const circumference = 2 * Math.PI * radius

/* вычисляемое свойство для stroke-dashoffset */
const strokeDashoffset = computed(() => {
    const progress = ssdUsage.value / 100
    return circumference * (1 - progress)
})

/* обновление данных */
const updateSSDData = (newTotal, newUsed) => {
    totalSSD.value = newTotal
    usedSSD.value = newUsed
}

// updateSSDData(80, 45)
</script>