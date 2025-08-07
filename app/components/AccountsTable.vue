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
          <th class="px-3 py-2.5 min-w-20"></th>
        </tr>
      </thead>
      <tbody>
        <tr class="border-b-[0.25px] border-[#ADADAD]">
          <td class="font-semibold pr-3 py-2.5">001</td>
          <td class="px-3 py-2.5">witty-tie</td>
          <td class="px-3 py-2.5">13 900</td>
          <td class="px-3 py-2.5">
            <div class="flex items-center gap-1 px-3 py-[3px] rounded-full bg-[#F0FEED] text-[#26C975] max-md:order-first w-fit shrink-0">
                <div class="w-1.5 h-1.5 rounded-full bg-[#26C975]"></div>
                <p class="text-[13px] font-medium leading-[100%]">Оплачен</p>
            </div>
          </td>
          <td class="px-3 py-2.5">12.06.2025</td>
          <td class="px-3 py-2.5 ">1 месяц</td>
          <td class="px-3 py-2.5 flex items-center gap-2 xl:grow xl:justify-end">
            <button class="cursor-pointer">
              <img src="/images/accounts/payment.svg" alt="" class="w-8">
            </button>
            <button class="cursor-pointer">
              <img src="/images/accounts/close.svg" alt="" class="w-8">
            </button>
            <button class="cursor-pointer">
              <img src="/images/accounts/list.svg" alt="" class="w-9">
            </button>
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</template> 
