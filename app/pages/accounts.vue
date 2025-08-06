<template>
    <section class="pt-9 pb-3.5 md:pb-6 grid-container bg-white">
        <div class="flex max-md:flex-col gap-3.5 md:justify-between md:items-center">
            <div class="flex flex-col gap-3">
                <p class="text-[28px] md:text-[32px] font-semibold leading-[100%]">Счета</p>
                <p class="text-[#ADADAD] text-sm leading-[100%]">Для корректного заполнения счета, пожалуйста заполните реквизиты в <a href="#" class="text-[#136BFB]">Профиле</a></p>
            </div>
            <div class="flex items-center gap-3.5 py-1.5 px-5 rounded-full bg-[#F7F7F7] w-fit">
                <label class="cursor-pointer">
                    <input type="date" class="sr-only">
                    <img src="/images/detail/date.png" alt="">
                </label>
                <p class="text-sm leading-[100%]">10.07.2025 - 16.07.2025</p>
            </div>
        </div>
    </section>
    <section class="pt-6 md:pt-8 pb-11 grid-container">
        <AccountsTable />
    </section>
</template>

<script setup>
</script>