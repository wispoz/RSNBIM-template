<template>
  <div class="w-full">
    <!-- Desktop & Tablet Version (sm and larger) -->
    <div class="hidden sm:block">
      <div class="bg-white rounded-lg shadow-sm border border-gray-100 overflow-hidden">
        <table class="w-full">
          <thead>
            <tr class="bg-gray-50 border-b border-gray-100">
              <th class="px-4 md:px-6 py-3 md:py-4 text-left text-sm font-medium text-gray-500">
                <span class="hidden md:inline">Номер</span>
                <span class="md:hidden">Номер/Сервер</span>
              </th>
              <th class="hidden md:table-cell px-6 py-4 text-left text-sm font-medium text-gray-500">Сервер</th>
              <th class="px-4 md:px-6 py-3 md:py-4 text-left text-sm font-medium text-gray-500">
                <span class="hidden md:inline">Цена, руб</span>
                <span class="md:hidden">Цена</span>
              </th>
              <th class="px-4 md:px-6 py-3 md:py-4 text-left text-sm font-medium text-gray-500">
                <div class="flex items-center gap-1 cursor-pointer">
                  <span class="hidden md:inline">Статус платежа</span>
                  <span class="md:hidden">Статус</span>
                  <img src="/images/detail/arrow.png" alt="sort" class="w-3 h-3">
                </div>
              </th>
              <th class="hidden md:table-cell px-6 py-4 text-left text-sm font-medium text-gray-500">
                <div class="flex items-center gap-1 cursor-pointer">
                  Дата создания
                  <img src="/images/detail/arrow.png" alt="sort" class="w-3 h-3">
                </div>
              </th>
              <th class="px-4 md:px-6 py-3 md:py-4 text-left text-sm font-medium text-gray-500">
                <span class="hidden md:inline">Период оплаты</span>
                <span class="md:hidden">Дата/Период</span>
              </th>
              <th class="px-4 md:px-6 py-3 md:py-4 text-right text-sm font-medium text-gray-500"></th>
            </tr>
          </thead>
          <tbody class="divide-y divide-gray-100">
            <!-- Row 1 - Paid -->
            <tr class="hover:bg-gray-50 transition-colors">
              <td class="px-4 md:px-6 py-3 md:py-4">
                <div class="md:hidden flex flex-col">
                  <span class="text-sm font-medium text-gray-900">001</span>
                  <span class="text-xs text-gray-500">witty-tie</span>
                </div>
                <span class="hidden md:inline text-sm font-medium text-gray-900">001</span>
              </td>
              <td class="hidden md:table-cell px-6 py-4 text-sm text-gray-900">witty-tie</td>
              <td class="px-4 md:px-6 py-3 md:py-4 text-sm font-medium text-gray-900">13 900</td>
              <td class="px-4 md:px-6 py-3 md:py-4">
                <span class="inline-flex items-center gap-1 px-2 md:px-3 py-1 md:py-1 rounded-full text-xs font-medium bg-green-100 text-green-800">
                  <span class="w-2 h-2 rounded-full bg-green-500"></span>
                  <span class="hidden md:inline">Оплачен</span>
                  <span class="md:hidden">Оплачен</span>
                </span>
              </td>
              <td class="hidden md:table-cell px-6 py-4 text-sm text-gray-600">12.06.2025</td>
              <td class="px-4 md:px-6 py-3 md:py-4">
                <div class="md:hidden flex flex-col">
                  <span class="text-sm text-gray-600">12.06.2025</span>
                  <span class="text-xs text-gray-500">1 месяц</span>
                </div>
                <span class="hidden md:inline text-sm text-gray-600">1 месяц</span>
              </td>
              <td class="px-4 md:px-6 py-3 md:py-4 text-right">
                <img src="/images/detail/icon1.svg" alt="details" class="w-5 h-5 text-gray-400 cursor-pointer hover:text-gray-600 ml-auto">
              </td>
            </tr>

            <!-- Row 2 - Pending -->
            <tr class="hover:bg-gray-50 transition-colors">
              <td class="px-4 md:px-6 py-3 md:py-4">
                <div class="md:hidden flex flex-col">
                  <span class="text-sm font-medium text-gray-900">002</span>
                  <span class="text-xs text-gray-500">witty-tie</span>
                </div>
                <span class="hidden md:inline text-sm font-medium text-gray-900">002</span>
              </td>
              <td class="hidden md:table-cell px-6 py-4 text-sm text-gray-900">witty-tie</td>
              <td class="px-4 md:px-6 py-3 md:py-4 text-sm font-medium text-gray-900">13 900</td>
              <td class="px-4 md:px-6 py-3 md:py-4">
                <span class="inline-flex items-center gap-1 px-2 md:px-3 py-1 md:py-1 rounded-full text-xs font-medium bg-red-100 text-red-800">
                  <span class="w-2 h-2 rounded-full bg-red-500"></span>
                  <span class="hidden md:inline">Ожидает оплаты</span>
                  <span class="md:hidden">Ожидает</span>
                </span>
              </td>
              <td class="hidden md:table-cell px-6 py-4 text-sm text-gray-600">12.06.2025</td>
              <td class="px-4 md:px-6 py-3 md:py-4">
                <div class="md:hidden flex flex-col">
                  <span class="text-sm text-gray-600">12.06.2025</span>
                  <span class="text-xs text-gray-500">1 месяц</span>
                </div>
                <span class="hidden md:inline text-sm text-gray-600">1 месяц</span>
              </td>
              <td class="px-4 md:px-6 py-3 md:py-4 text-right">
                <div class="flex items-center justify-end gap-2 max-lg:flex-col">
                  <div class="flex gap-1 md:gap-2 max-lg:order-last">
                    <button class="px-3 md:px-4 py-1.5 md:py-2 bg-blue-600 text-white text-xs md:text-sm font-medium rounded md:rounded-lg hover:bg-blue-700 transition-colors">
                      Оплатить
                    </button>
                    <button class="px-3 md:px-4 py-1.5 md:py-2 bg-red-600 text-white text-xs md:text-sm font-medium rounded md:rounded-lg hover:bg-red-700 transition-colors">
                      Отмена
                    </button>
                  </div>
                  <img src="/images/detail/icon1.svg" alt="details" class="w-5 h-5 text-gray-400 cursor-pointer hover:text-gray-600">
                </div>
              </td>
            </tr>

            <!-- Row 3 - Canceled -->
            <tr class="hover:bg-gray-50 transition-colors">
              <td class="px-4 md:px-6 py-3 md:py-4">
                <div class="md:hidden flex flex-col">
                  <span class="text-sm font-medium text-gray-900">003</span>
                  <span class="text-xs text-gray-500">Dev_serv</span>
                </div>
                <span class="hidden md:inline text-sm font-medium text-gray-900">003</span>
              </td>
              <td class="hidden md:table-cell px-6 py-4 text-sm text-gray-900">Dev_serv</td>
              <td class="px-4 md:px-6 py-3 md:py-4 text-sm font-medium text-gray-900">13 900</td>
              <td class="px-4 md:px-6 py-3 md:py-4">
                <span class="inline-flex items-center gap-1 px-2 md:px-3 py-1 md:py-1 rounded-full text-xs font-medium bg-gray-100 text-gray-800">
                  <span class="w-2 h-2 rounded-full bg-gray-500"></span>
                  <span class="hidden md:inline">Отменен</span>
                  <span class="md:hidden">Отменен</span>
                </span>
              </td>
              <td class="hidden md:table-cell px-6 py-4 text-sm text-gray-600">12.06.2025</td>
              <td class="px-4 md:px-6 py-3 md:py-4">
                <div class="md:hidden flex flex-col">
                  <span class="text-sm text-gray-600">12.06.2025</span>
                  <span class="text-xs text-gray-500">1 месяц</span>
                </div>
                <span class="hidden md:inline text-sm text-gray-600">1 месяц</span>
              </td>
              <td class="px-4 md:px-6 py-3 md:py-4 text-right">
                <img src="/images/detail/icon1.svg" alt="details" class="w-5 h-5 text-gray-400 cursor-pointer hover:text-gray-600 ml-auto">
              </td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>

    <!-- Mobile Version (xs to sm) -->
    <div class="block sm:hidden">
      <div class="space-y-3">
        <!-- Card 1 - Paid -->
        <div class="bg-white rounded-lg shadow-sm border border-gray-100 p-4">
          <div class="flex justify-between items-start mb-3">
            <div class="flex-1">
              <div class="flex items-center gap-2 mb-2">
                <span class="text-sm font-medium text-gray-900">001</span>
                <span class="text-sm text-gray-900">witty-tie</span>
              </div>
              <div class="flex items-center gap-4 text-xs text-gray-500">
                <span>12.06.2025</span>
                <span>1 месяц</span>
              </div>
            </div>
            <div class="text-right">
              <div class="text-lg font-semibold text-gray-900 mb-2">13 900</div>
              <span class="inline-flex items-center gap-1 px-3 py-1 rounded-full text-xs font-medium bg-green-100 text-green-800">
                <span class="w-2 h-2 rounded-full bg-green-500"></span>
                Оплачен
              </span>
            </div>
          </div>
          <div class="flex items-center justify-between">
            <img src="/images/detail/icon1.svg" alt="details" class="w-5 h-5 text-gray-400 cursor-pointer hover:text-gray-600 ml-auto">
          </div>
        </div>

        <!-- Card 2 - Pending -->
        <div class="bg-white rounded-lg shadow-sm border border-gray-100 p-4">
          <div class="flex justify-between items-start mb-3">
            <div class="flex-1">
              <div class="flex items-center gap-2 mb-2">
                <span class="text-sm font-medium text-gray-900">002</span>
                <span class="text-sm text-gray-900">witty-tie</span>
              </div>
              <div class="flex items-center gap-4 text-xs text-gray-500">
                <span>12.06.2025</span>
                <span>1 месяц</span>
              </div>
            </div>
            <div class="text-right">
              <div class="text-lg font-semibold text-gray-900 mb-2">13 900</div>
              <span class="inline-flex items-center gap-1 px-3 py-1 rounded-full text-xs font-medium bg-red-100 text-red-800">
                <span class="w-2 h-2 rounded-full bg-red-500"></span>
                Ожидает оплаты
              </span>
            </div>
          </div>
          <div class="flex items-center justify-between">
            <div class="flex gap-2">
              <button class="px-4 py-2 bg-blue-600 text-white text-sm font-medium rounded-lg hover:bg-blue-700 transition-colors">
                Оплатить
              </button>
              <button class="px-4 py-2 bg-red-600 text-white text-sm font-medium rounded-lg hover:bg-red-700 transition-colors">
                Отмена
              </button>
            </div>
            <img src="/images/detail/icon1.svg" alt="details" class="w-5 h-5 text-gray-400 cursor-pointer hover:text-gray-600 ml-auto">
          </div>
        </div>

        <!-- Card 3 - Canceled -->
        <div class="bg-white rounded-lg shadow-sm border border-gray-100 p-4">
          <div class="flex justify-between items-start mb-3">
            <div class="flex-1">
              <div class="flex items-center gap-2 mb-2">
                <span class="text-sm font-medium text-gray-900">003</span>
                <span class="text-sm text-gray-900">Dev_serv</span>
              </div>
              <div class="flex items-center gap-4 text-xs text-gray-500">
                <span>12.06.2025</span>
                <span>1 месяц</span>
              </div>
            </div>
            <div class="text-right">
              <div class="text-lg font-semibold text-gray-900 mb-2">13 900</div>
              <span class="inline-flex items-center gap-1 px-3 py-1 rounded-full text-xs font-medium bg-gray-100 text-gray-800">
                <span class="w-2 h-2 rounded-full bg-gray-500"></span>
                Отменен
              </span>
            </div>
          </div>
          <div class="flex items-center justify-between">
            <img src="/images/detail/icon1.svg" alt="details" class="w-5 h-5 text-gray-400 cursor-pointer hover:text-gray-600 ml-auto">
          </div>
        </div>
      </div>
    </div>
  </div>
</template> 