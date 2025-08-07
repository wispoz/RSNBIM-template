<template>
    <section class="pt-9 pb-3.5 md:pb-6 grid-container bg-white">
        <div class="flex max-md:flex-col gap-3.5 md:justify-between md:items-center">
            <div class="flex flex-col gap-3">
                <p class="text-[28px] md:text-[32px] font-semibold leading-[100%]">Счета</p>
                <p class="text-[#ADADAD] text-sm leading-[100%]">Для корректного заполнения счета, пожалуйста заполните реквизиты в <a href="#" class="text-[#136BFB]">Профиле</a></p>
            </div>
            <div class="flex items-center gap-3.5 py-1.5 px-5 rounded-full bg-[#F7F7F7] w-fit shrink-0">
                <label class="cursor-pointer">
                    <input type="date" class="sr-only">
                    <img src="/images/detail/date.png" alt="">
                </label>
                <p class="text-sm leading-[100%]">10.07.2025 - 16.07.2025</p>
            </div>
        </div>
    </section>
    <section class="pt-6 md:pt-8 pb-11 grid-container">
        <div class="w-full bg-white rounded-[15px] overflow-hidden py-2.5 px-5 text-xs leading-[100%] max-md:col-span-full">
            <table class="w-full max-md:hidden">
            <thead>
                <tr class="border-b-[0.25px] border-[#ADADAD] text-[#ADADAD] text-left">
                <th class="pr-3 py-2.5 font-normal">Номер</th>
                <th class="px-3 py-2.5 font-normal">Сервер</th>
                <th class="px-3 py-2.5 font-normal">Цена, руб</th>
                <th class="px-3 py-2.5 font-normal">
                    <button class="flex items-center gap-1">
                    <span>Статус платежа</span>
                    <img src="/images/accounts/arrow.png" alt="">
                    </button>
                </th>
                <th class="px-3 py-2.5 font-normal">
                    <button class="flex items-center gap-1">
                    <span>Дата создания</span>
                    <img src="/images/accounts/arrow.png" alt="">
                    </button>
                </th>
                <th class="px-3 py-2.5 font-normal">Период оплаты</th>
                <th class="px-3 py-2.5 min-w-20"></th>
                </tr>
            </thead>
            <tbody>
                <tr class="border-b-[0.25px] border-[#ADADAD] last:border-none">
                <td class="font-semibold pr-3 py-2.5">001</td>
                <td class="px-3 py-2.5">witty-tie</td>
                <td class="px-3 py-2.5">13 900</td>
                <td class="px-3 py-2.5">
                    <div class="flex items-center gap-1 px-3 py-[3px] rounded-full bg-[#F0FEED] text-[#26C975] w-fit shrink-0">
                        <div class="w-1.5 h-1.5 rounded-full bg-[#26C975]"></div>
                        <p class="text-[13px] font-medium leading-[100%]">Оплачен</p>
                    </div>
                </td>
                <td class="px-3 py-2.5">12.06.2025</td>
                <td class="px-3 py-2.5 ">1 месяц</td>
                <td class="px-3 py-2.5 flex items-center md:grow md:justify-end">
                    <button class="cursor-pointer relative group">
                        <img src="/images/accounts/list.svg" alt="" class="w-8">
                        <span class="absolute left-1/2 -translate-x-1/2 -top-8 px-2 py-1 rounded bg-[#0F0F0F] text-white text-xs opacity-0 group-hover:opacity-100 pointer-events-none transition-all duration-500 whitespace-nowrap z-[1]">
                            Скачать
                        </span>
                    </button>
                </td>
                </tr>
                <tr class="border-b-[0.25px] border-[#ADADAD] last:border-none">
                <td class="font-semibold pr-3 py-2.5">001</td>
                <td class="px-3 py-2.5">witty-tie</td>
                <td class="px-3 py-2.5">13 900</td>
                <td class="px-3 py-2.5">
                    <div class="flex items-center gap-1 px-3 py-[3px] rounded-full bg-[#FDF1F2] text-[#FF6170] w-fit shrink-0">
                        <div class="w-1.5 h-1.5 rounded-full bg-[#FF6170]"></div>
                        <p class="text-[13px] font-medium leading-[100%]">Ожидает оплаты</p>
                    </div>
                </td>
                <td class="px-3 py-2.5">12.06.2025</td>
                <td class="px-3 py-2.5 ">1 месяц</td>
                <td class="px-3 py-2.5 flex items-center gap-2 md:grow md:justify-end">
                    <button class="cursor-pointer relative group">
                        <img src="/images/accounts/payment.svg" alt="" class="w-8">
                        <span class="absolute left-1/2 -translate-x-1/2 -top-8 px-2 py-1 rounded bg-[#0F0F0F] text-white text-xs opacity-0 group-hover:opacity-100 pointer-events-none transition-all duration-500 whitespace-nowrap z-[1]">
                            Оплатить
                        </span>
                    </button>
                    <button class="cursor-pointer relative group">
                        <img src="/images/accounts/close.svg" alt="" class="w-8">
                        <span class="absolute left-1/2 -translate-x-1/2 -top-8 px-2 py-1 rounded bg-[#0F0F0F] text-white text-xs opacity-0 group-hover:opacity-100 pointer-events-none transition-all duration-500 whitespace-nowrap z-[1]">
                            Отменить
                        </span>
                    </button>
                    <button class="cursor-pointer relative group">
                        <img src="/images/accounts/list.svg" alt="" class="w-8">
                        <span class="absolute left-1/2 -translate-x-1/2 -top-8 px-2 py-1 rounded bg-[#0F0F0F] text-white text-xs opacity-0 group-hover:opacity-100 pointer-events-none transition-all duration-500 whitespace-nowrap z-[1]">
                            Скачать
                        </span>
                    </button>
                </td>
                </tr>
                <tr class="border-b-[0.25px] border-[#ADADAD] last:border-none">
                <td class="font-semibold pr-3 py-2.5">001</td>
                <td class="px-3 py-2.5">witty-tie</td>
                <td class="px-3 py-2.5">13 900</td>
                <td class="px-3 py-2.5">
                    <div class="flex items-center gap-1 px-3 py-[3px] rounded-full bg-[#F7F7F7] text-[#ADADAD] w-fit shrink-0">
                        <div class="w-1.5 h-1.5 rounded-full bg-[#ADADAD]"></div>
                        <p class="text-[13px] font-medium leading-[100%]">Отменен</p>
                    </div>
                </td>
                <td class="px-3 py-2.5">12.06.2025</td>
                <td class="px-3 py-2.5 ">1 месяц</td>
                <td class="px-3 py-2.5 flex items-center md:grow md:justify-end">
                    <button class="cursor-pointer relative group">
                        <img src="/images/accounts/list.svg" alt="" class="w-8">
                        <span class="absolute left-1/2 -translate-x-1/2 -top-8 px-2 py-1 rounded bg-[#0F0F0F] text-white text-xs opacity-0 group-hover:opacity-100 pointer-events-none transition-all duration-500 whitespace-nowrap z-[1]">
                            Скачать
                        </span>
                    </button>
                </td>
                </tr>
            </tbody>
            </table>
            <div class="md:hidden flex flex-col gap-3.5 text-xs leading-[100%]">
            <div class="flex flex-col gap-2.5">
                <div class="flex items-center justify-between">
                <div class="flex items-center gap-2.5">
                    <p class="font-semibold">001</p>
                    <p class="font-semibold text-base">witty-tie</p>
                </div>
                <p class="font-semibold text-base">13 900</p>
                </div>
                <div class="flex items-center justify-between">
                <p class="text-[#ADADAD]">12.06.2025</p>
                <div class="flex items-center gap-1 px-3 py-[3px] rounded-full bg-[#F0FEED] text-[#26C975] w-fit shrink-0">
                    <div class="w-1.5 h-1.5 rounded-full bg-[#26C975]"></div>
                    <p class="text-[13px] font-medium leading-[100%]">Оплачен</p>
                </div>
                </div>
                <div class="flex flex-col w-full">
                <p class="text-[#ADADAD]">1 месяц</p>
                <div class="flex items-center gap-2.5 justify-end">
                    <button class="cursor-pointer">
                    <img src="/images/accounts/list.svg" alt="" class="w-9">
                    </button>
                </div>
                </div>
            </div>
            <div class="w-full h-[0.25px] bg-[#ADADAD] last:hidden"></div>
            <div class="flex flex-col gap-2.5">
                <div class="flex items-center justify-between">
                <div class="flex items-center gap-2.5">
                    <p class="font-semibold">001</p>
                    <p class="font-semibold text-base">witty-tie</p>
                </div>
                <p class="font-semibold text-base">13 900</p>
                </div>
                <div class="flex items-center justify-between">
                <p class="text-[#ADADAD]">12.06.2025</p>
                <div class="flex items-center gap-1 px-3 py-[3px] rounded-full bg-[#FDF1F2] text-[#FF6170] w-fit shrink-0">
                    <div class="w-1.5 h-1.5 rounded-full bg-[#FF6170]"></div>
                    <p class="text-[13px] font-medium leading-[100%]">Ожидает оплаты</p>
                </div>
                </div>
                <div class="flex flex-col w-full">
                <p class="text-[#ADADAD]">1 месяц</p>
                <div class="flex items-center gap-2.5 justify-end">
                    <button class="cursor-pointer">
                    <img src="/images/accounts/payment.svg" alt="" class="w-8">
                    </button>
                    <button class="cursor-pointer">
                    <img src="/images/accounts/close.svg" alt="" class="w-8">
                    </button>
                    <button class="cursor-pointer">
                    <img src="/images/accounts/list.svg" alt="" class="w-9">
                    </button>
                </div>
                </div>
            </div>
            <div class="w-full h-[0.25px] bg-[#ADADAD] last:hidden"></div>
            <div class="flex flex-col gap-2.5">
                <div class="flex items-center justify-between">
                <div class="flex items-center gap-2.5">
                    <p class="font-semibold">001</p>
                    <p class="font-semibold text-base">witty-tie</p>
                </div>
                <p class="font-semibold text-base">13 900</p>
                </div>
                <div class="flex items-center justify-between">
                <p class="text-[#ADADAD]">12.06.2025</p>
                <div class="flex items-center gap-1 px-3 py-[3px] rounded-full bg-[#F7F7F7] text-[#ADADAD] w-fit shrink-0">
                    <div class="w-1.5 h-1.5 rounded-full bg-[#ADADAD]"></div>
                    <p class="text-[13px] font-medium leading-[100%]">Отменен</p>
                </div>
                </div>
                <div class="flex flex-col w-full">
                <p class="text-[#ADADAD]">1 месяц</p>
                <div class="flex items-center gap-2.5 justify-end">
                    <button class="cursor-pointer">
                    <img src="/images/accounts/list.svg" alt="" class="w-9">
                    </button>
                </div>
                </div>
            </div>
            </div>
        </div>
    </section>
</template>

<script setup>
</script>