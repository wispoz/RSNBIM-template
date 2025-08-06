<template>
  <div class="w-full bg-white rounded-[15px] overflow-hidden py-2.5 px-5 text-xs leading-[100%]">
    <table class="w-full">
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
        </tr>
      </thead>
      <tbody>
        <tr class="border-b-[0.25px] border-[#ADADAD]">
          <td class="font-semibold pr-3 py-2.5 align-top">001</td>
          <td class="px-3 py-2.5 align-top">witty-tie</td>
          <td class="px-3 py-2.5 align-top">13 900</td>
          <td class="px-3 py-2.5 align-top">
            <div class="flex items-center gap-1 px-3 py-[3px] rounded-full bg-[#F0FEED] text-[#26C975] max-md:order-first w-fit shrink-0">
                <div class="w-1.5 h-1.5 rounded-full bg-[#26C975]"></div>
                <p class="text-[13px] font-medium leading-[100%]">Оплачен</p>
            </div>
          </td>
          <td class="px-3 py-2.5 align-top">12.06.2025</td>
          <td class="px-3 py-2.5 flex gap-6 xl:gap-20">
            <span class="shrink-0">1 месяц</span>
            <div class="flex items-center gap-2 max-xl:items-end max-xl:flex-col">
              <div class="flex items-center gap-2 max-xl:order-last">
                <button class="flex items-center justify-center w-[101px] h-[31px] text-sm font-semibold text-white rounded-full bg-[#136BFB]">Оплатить</button>
                <button class="flex items-center justify-center w-[101px] h-[31px] text-sm font-semibold text-white rounded-full bg-[#FF6170]">Отмена</button>
              </div>
              <button class="cursor-pointer">
                <img src="/images/accounts/list.png" alt="" class="shrink-0">
              </button>
            </div>
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</template> 
