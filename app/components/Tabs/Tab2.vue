<template>
    <div class="flex flex-col gap-6 md:gap-4">
        <div class="flex items-center justify-between gap-0.5 text-sm leading-[100%]">
            <button class="flex items-center justify-center w-[107px] md:w-[137px] gap-1.5 md:gap-4 py-2 rounded-2xl bg-[#136BFB] text-white font-semibold">
                <img src="/images/detail/plus.png" alt="">
                <span>Добавить</span>
            </button>
            <p>Ваш IP: 5.35.115.54</p>
        </div>
        
        <div class="bg-white rounded-[20px] px-5 xl:px-6 pt-2.5 pb-7 max-md:hidden">
            <table class="w-full text-sm leading-[100%]">
                <thead>
                    <tr class="border-b-[0.5px] border-[#ADADAD] text-left text-[#ADADAD]">
                        <th class="py-4 px-2">Название</th> 
                        <th class="py-4 px-2">IP</th> 
                        <th class="py-4 px-2">Дата</th> 
                    </tr>
                </thead>
                <!-- <tbody>
                    <tr class="border-b-[0.5px] border-[#ADADAD]">
                        <td class="py-4 px-2 font-semibold">Название</td>
                        <td class="py-4 px-2">5.35.115.54</td>
                        <td class="py-4 px-2">12.06.2025</td>
                    </tr>
                </tbody> -->
            </table>
            <div class="flex items-center justify-center py-16">
                <p class="text-sm leading-[100%] text-[#ADADAD]">Revit Server доступен всем</p>
            </div>
        </div>

        <div class="flex flex-col gap-3 md:hidden text-sm leading-[100%]">
            <div class="flex flex-col gap-2.5 group">
                <div class="flex items-center justify-between">
                    <p class="font-semibold">Название текст</p>
                    <div class="flex items-center gap-3">
                        <button class="cursor-pointer">
                            <img src="/images/detail/edit.png" alt="">
                        </button>
                        <button class="cursor-pointer">
                            <img src="/images/detail/delete.png" alt="">
                        </button>
                    </div>
                </div>
                <div class="flex items-center justify-between">
                    <p>IP: 5.35.115.54</p>
                    <p class="text-[#ADADAD]">12.06.2025</p>
                </div>
                <div class="w-full h-[0.5px] bg-[#ADADAD] group-last:hidden"></div>
            </div>
            <div class="flex flex-col gap-2.5 group">
                <div class="flex items-center justify-between">
                    <p class="font-semibold">Название текст</p>
                    <div class="flex items-center gap-3">
                        <button class="cursor-pointer">
                            <img src="/images/detail/edit.png" alt="">
                        </button>
                        <button class="cursor-pointer">
                            <img src="/images/detail/delete.png" alt="">
                        </button>
                    </div>
                </div>
                <div class="flex items-center justify-between">
                    <p>IP: 5.35.115.54</p>
                    <p class="text-[#ADADAD]">12.06.2025</p>
                </div>
                <div class="w-full h-[0.5px] bg-[#ADADAD] group-last:hidden"></div>
            </div>
            <div class="flex flex-col gap-2.5 group">
                <div class="flex items-center justify-between">
                    <p class="font-semibold">Название текст</p>
                    <div class="flex items-center gap-3">
                        <button class="cursor-pointer">
                            <img src="/images/detail/edit.png" alt="">
                        </button>
                        <button class="cursor-pointer">
                            <img src="/images/detail/delete.png" alt="">
                        </button>
                    </div>
                </div>
                <div class="flex items-center justify-between">
                    <p>IP: 5.35.115.54</p>
                    <p class="text-[#ADADAD]">12.06.2025</p>
                </div>
                <div class="w-full h-[0.5px] bg-[#ADADAD] group-last:hidden"></div>
            </div>
            <div class="flex flex-col gap-2.5 group">
                <div class="flex items-center justify-between">
                    <p class="font-semibold">Название текст</p>
                    <div class="flex items-center gap-3">
                        <button class="cursor-pointer">
                            <img src="/images/detail/edit.png" alt="">
                        </button>
                        <button class="cursor-pointer">
                            <img src="/images/detail/delete.png" alt="">
                        </button>
                    </div>
                </div>
                <div class="flex items-center justify-between">
                    <p>IP: 5.35.115.54</p>
                    <p class="text-[#ADADAD]">12.06.2025</p>
                </div>
                <div class="w-full h-[0.5px] bg-[#ADADAD] group-last:hidden"></div>
            </div>
        </div>
    </div>
</template>

<script setup>

</script>