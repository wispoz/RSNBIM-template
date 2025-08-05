<template>
    <div class="flex flex-col">
        <div class="flex items-center max-md:flex-wrap gap-2.5 md:gap-1 max-md:text-[#ADADAD] text-sm font-medium leading-[100%]">
            <button @click="activeTab = 'tab1'" :class="{'!bg-[#136BFB] max-md:!text-white md:!bg-white md:!border-white' : activeTab === 'tab1'}" class="cursor-pointer transition-all duration-500 text-center max-md:rounded-full md:rounded-t-[20px] py-1.5 md:pt-2.5 md:pb-4 w-[134px] md:w-[139px] bg-white md:bg-transparent md:border border-[#E2E2E2]">Отчет</button>
            <button @click="activeTab = 'tab2'" :class="{'!bg-[#136BFB] max-md:!text-white md:!bg-white md:!border-white' : activeTab === 'tab2'}" class="cursor-pointer transition-all duration-500 text-center max-md:rounded-full md:rounded-t-[20px] py-1.5 md:pt-2.5 md:pb-4 w-[134px] md:w-[139px] bg-white md:bg-transparent md:border border-[#E2E2E2]">Пользователи</button>
        </div>
        <div class="rounded-[14px] md:rounded-tl-none bg-white max-md:mt-4 px-4 py-5 md:py-4 xl:px-6">
            <div v-show="activeTab === 'tab1'" class="flex flex-col gap-6 md:gap-8 w-full">
                <div class="flex flex-col gap-4">
                    <div class="flex items-center gap-3.5 py-1.5 px-5 rounded-full bg-[#F7F7F7] w-fit">
                        <label class="cursor-pointer">
                            <input type="date" class="sr-only">
                            <img src="/images/detail/date.png" alt="">
                        </label>
                        <p class="text-sm leading-[100%]">10.07.2025 - 16.07.2025</p>
                    </div>
                </div>
                <div class="grid grid-cols-2 md:grid-cols-4 gap-1 md:gap-2">
                    <div class="flex flex-col gap-1 rounded-[10px] px-2 pt-1.5 pb-3.5 md:px-5 md:pt-2 md:pb-3 text-white bg-[#136BFB]">
                        <div class="flex items-center justify-between">
                            <p class="text-[20px] md:text-[30px] font-semibold leading-[100%]">100</p>
                            <img src="/images/detail/clock_new.png" alt="">
                        </div>
                        <p class="text-sm md:text-lg font-semibold leading-[100%]">Отработанное время</p>
                    </div>
                    <div class="flex flex-col gap-1 rounded-[10px] px-2 pt-1.5 pb-3.5 md:px-5 md:pt-2 md:pb-3 text-white bg-[#26C975]">
                        <div class="flex items-center justify-between">
                            <p class="text-[20px] md:text-[30px] font-semibold leading-[100%]">30</p>
                            <img src="/images/detail/add_new.png" alt="">
                        </div>
                        <p class="text-sm md:text-lg font-semibold leading-[100%]">Созданных элементов</p>
                    </div>
                    <div class="flex flex-col gap-1 rounded-[10px] px-2 pt-1.5 pb-3.5 md:px-5 md:pt-2 md:pb-3 text-white bg-[#EFB000]">
                        <div class="flex items-center justify-between">
                            <p class="text-[20px] md:text-[30px] font-semibold leading-[100%]">30</p>
                            <img src="/images/detail/edit_new.png" alt="">
                        </div>
                        <p class="text-sm md:text-lg font-semibold leading-[100%]">Измененных элементов</p>
                    </div>
                    <div class="flex flex-col gap-1 rounded-[10px] px-2 pt-1.5 pb-3.5 md:px-5 md:pt-2 md:pb-3 text-white bg-[#FF6170]">
                        <div class="flex items-center justify-between">
                            <p class="text-[20px] md:text-[30px] font-semibold leading-[100%]">10</p>
                            <img src="/images/detail/del_new.png" alt="">
                        </div>
                        <p class="text-sm md:text-lg font-semibold leading-[100%]">Удаленных элементов</p>
                    </div>
                </div>

                <!-- Chart -->
                <div>
                    <div class="relative h-[430px] md:h-[300px]">
                        <canvas ref="chartRef"></canvas>
                    </div>
                </div>

                <div class="max-md:hidden text-sm leading-[100%]">
                    <table class="w-full">
                        <thead>
                            <tr class="border-b-[0.5px] border-[#ADADAD]">
                                <th class="py-3 px-2 font-normal text-left"></th>
                                <th class="py-3 px-2 font-normal text-left">10.07.25</th>
                                <th class="py-3 px-2 font-normal text-left">11.07.25</th>
                                <th class="py-3 px-2 font-normal text-left">12.07.25</th>
                                <th class="py-3 px-2 font-normal text-left">13.07.25</th>
                                <th class="py-3 px-2 font-normal text-left">14.07.25</th>
                                <th class="py-3 px-2 font-normal text-left">15.07.25</th>
                                <th class="py-3 px-2 font-normal text-left">16.07.25</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr class="border-b-[0.5px] border-[#ADADAD] last:border-none">
                                <td class="py-3 px-2 font-semibold">Отработанное время</td>
                                <td class="py-3 px-2">110</td>
                                <td class="py-3 px-2">110</td>
                                <td class="py-3 px-2">110</td>
                                <td class="py-3 px-2">110</td>
                                <td class="py-3 px-2">110</td>
                                <td class="py-3 px-2">110</td>
                                <td class="py-3 px-2">110</td>
                            </tr>
                            <tr class="border-b-[0.5px] border-[#ADADAD] last:border-none">
                                <td class="py-3 px-2 font-semibold">Созданных элементов</td>
                                <td class="py-3 px-2">45</td>
                                <td class="py-3 px-2">45</td>
                                <td class="py-3 px-2">45</td>
                                <td class="py-3 px-2">45</td>
                                <td class="py-3 px-2">45</td>
                                <td class="py-3 px-2">45</td>
                                <td class="py-3 px-2">45</td>
                            </tr>
                            <tr class="border-b-[0.5px] border-[#ADADAD] last:border-none">
                                <td class="py-3 px-2 font-semibold">Измененных элементов</td>
                                <td class="py-3 px-2">20</td>
                                <td class="py-3 px-2">20</td>
                                <td class="py-3 px-2">20</td>
                                <td class="py-3 px-2">20</td>
                                <td class="py-3 px-2">20</td>
                                <td class="py-3 px-2">20</td>
                                <td class="py-3 px-2">20</td>
                            </tr>
                            <tr class="border-b-[0.5px] border-[#ADADAD] last:border-none">
                                <td class="py-3 px-2 font-semibold">Удаленных элементов</td>
                                <td class="py-3 px-2">5</td>
                                <td class="py-3 px-2">5</td>
                                <td class="py-3 px-2">5</td>
                                <td class="py-3 px-2">5</td>
                                <td class="py-3 px-2">5</td>
                                <td class="py-3 px-2">5</td>
                                <td class="py-3 px-2">5</td>
                            </tr>
                        </tbody>
                    </table>
                </div>

                <div class="md:hidden space-y-3">
                    <div class="flex flex-col gap-1.5">
                        <p class="text-sm text-[#ADADAD]">10.07.25</p>
                        <div class="grid grid-cols-[74%_26%] gap-x-4 gap-y-1.5 text-xs leading-[100%]">
                            <p class="font-semibold">Отработанное время</p>
                            <p class="font-semibold">110</p>
                            <p class="font-semibold">Созданных элементов</p>
                            <p class="font-semibold">45</p>
                            <p class="font-semibold">Измененных элементов</p>
                            <p class="font-semibold">20</p>
                            <p class="font-semibold">Удаленных элементов</p>
                            <p class="font-semibold">5</p>
                        </div>
                    </div>
                    <div class="w-full h-[0.5px] bg-[#ADADAD]"></div>
                    <div class="flex flex-col gap-1.5">
                        <p class="text-sm text-[#ADADAD]">11.07.25</p>
                        <div class="grid grid-cols-[74%_26%] gap-x-4 gap-y-1.5 text-xs leading-[100%]">
                            <p class="font-semibold">Отработанное время</p>
                            <p class="font-semibold">110</p>
                            <p class="font-semibold">Созданных элементов</p>
                            <p class="font-semibold">45</p>
                            <p class="font-semibold">Измененных элементов</p>
                            <p class="font-semibold">20</p>
                            <p class="font-semibold">Удаленных элементов</p>
                            <p class="font-semibold">5</p>
                        </div>
                    </div>
                    <div class="w-full h-[0.5px] bg-[#ADADAD]"></div>
                    <div class="flex flex-col gap-1.5">
                        <p class="text-sm text-[#ADADAD]">12.07.25</p>
                        <div class="grid grid-cols-[74%_26%] gap-x-4 gap-y-1.5 text-xs leading-[100%]">
                            <p class="font-semibold">Отработанное время</p>
                            <p class="font-semibold">110</p>
                            <p class="font-semibold">Созданных элементов</p>
                            <p class="font-semibold">45</p>
                            <p class="font-semibold">Измененных элементов</p>
                            <p class="font-semibold">20</p>
                            <p class="font-semibold">Удаленных элементов</p>
                            <p class="font-semibold">5</p>
                        </div>
                    </div>
                    <div class="w-full h-[0.5px] bg-[#ADADAD]"></div>
                    <div class="flex flex-col gap-1.5">
                        <p class="text-sm text-[#ADADAD]">13.07.25</p>
                        <div class="grid grid-cols-[74%_26%] gap-x-4 gap-y-1.5 text-xs leading-[100%]">
                            <p class="font-semibold">Отработанное время</p>
                            <p class="font-semibold">110</p>
                            <p class="font-semibold">Созданных элементов</p>
                            <p class="font-semibold">45</p>
                            <p class="font-semibold">Измененных элементов</p>
                            <p class="font-semibold">20</p>
                            <p class="font-semibold">Удаленных элементов</p>
                            <p class="font-semibold">5</p>
                        </div>
                    </div>
                    <div class="w-full h-[0.5px] bg-[#ADADAD]"></div>
                    <div class="flex flex-col gap-1.5">
                        <p class="text-sm text-[#ADADAD]">14.07.25</p>
                        <div class="grid grid-cols-[74%_26%] gap-x-4 gap-y-1.5 text-xs leading-[100%]">
                            <p class="font-semibold">Отработанное время</p>
                            <p class="font-semibold">110</p>
                            <p class="font-semibold">Созданных элементов</p>
                            <p class="font-semibold">45</p>
                            <p class="font-semibold">Измененных элементов</p>
                            <p class="font-semibold">20</p>
                            <p class="font-semibold">Удаленных элементов</p>
                            <p class="font-semibold">5</p>
                        </div>
                    </div>
                    <div class="w-full h-[0.5px] bg-[#ADADAD]"></div>
                    <div class="flex flex-col gap-1.5">
                        <p class="text-sm text-[#ADADAD]">15.07.25</p>
                        <div class="grid grid-cols-[74%_26%] gap-x-4 gap-y-1.5 text-xs leading-[100%]">
                            <p class="font-semibold">Отработанное время</p>
                            <p class="font-semibold">110</p>
                            <p class="font-semibold">Созданных элементов</p>
                            <p class="font-semibold">45</p>
                            <p class="font-semibold">Измененных элементов</p>
                            <p class="font-semibold">20</p>
                            <p class="font-semibold">Удаленных элементов</p>
                            <p class="font-semibold">5</p>
                        </div>
                    </div>
                    <div class="w-full h-[0.5px] bg-[#ADADAD]"></div>
                    <div class="flex flex-col gap-1.5">
                        <p class="text-sm text-[#ADADAD]">16.07.25</p>
                        <div class="grid grid-cols-[74%_26%] gap-x-4 gap-y-1.5 text-xs leading-[100%]">
                            <p class="font-semibold">Отработанное время</p>
                            <p class="font-semibold">110</p>
                            <p class="font-semibold">Созданных элементов</p>
                            <p class="font-semibold">45</p>
                            <p class="font-semibold">Измененных элементов</p>
                            <p class="font-semibold">20</p>
                            <p class="font-semibold">Удаленных элементов</p>
                            <p class="font-semibold">5</p>
                        </div>
                    </div>
                </div>
            </div>
            <div v-show="activeTab === 'tab2'" class="flex flex-col gap-6 md:gap-5">
                <button class="flex items-center justify-center w-[107px] md:w-[137px] gap-1.5 md:gap-4 py-2 rounded-full bg-[#136BFB] text-white font-semibold">
                    <img src="/images/detail/plus.png" alt="">
                    <span class="text-sm font-semibold leading-[100%]">Добавить</span>
                </button>

                <div class="max-md:hidden">
                    <table class="w-full text-sm leading-[100%]">
                        <thead>
                            <tr class="border-b-[0.5px] border-[#ADADAD] text-left text-[#ADADAD]">
                                <th class="py-4 px-2 font-normal">Название</th> 
                                <th class="py-4 px-2 font-normal">E-mail</th> 
                                <th class="py-4 px-2 font-normal">Токен</th> 
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
                        <p class="text-sm leading-[100%] text-[#ADADAD]">Записей нет </p>
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
                        <div class="flex items-start justify-between">
                            <p class="max-w-[132px]">E-mail@mail.ru</p>
                            <p class="text-[#ADADAD]">12.06.2025</p>
                        </div>
                        <p>Токен 000000</p>
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
                        <div class="flex items-start justify-between">
                            <p class="max-w-[132px]">E-mail@mail.ru</p>
                            <p class="text-[#ADADAD]">12.06.2025</p>
                        </div>
                        <p>Токен 000000</p>
                        <div class="w-full h-[0.5px] bg-[#ADADAD] group-last:hidden"></div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { Chart, registerables } from 'chart.js'

/* код табов */
const activeTab = ref('tab1')

/* регистрирация всех компонентов Chart.js */
Chart.register(...registerables)

/* ссылки на canvas элементы */
const chartRef = ref(null)

/* данные для диаграммы */
const chartData = {
    labels: ['10.07.25', '11.07.25', '12.07.25', '13.07.25', '14.07.25', '15.07.25', '16.07.25'],
    datasets: [
        {
            label: 'Отработанное время',
            data: [102, 87, 42, 42, 47, 77, 47],
            backgroundColor: '#136BFB',
            borderColor: '#136BFB',
            borderWidth: 0,
            borderRadius: 6,
            borderSkipped: false,
        },
        {
            label: 'Созданных элементов',
            data: [47, 13, 27, 38, 27, 27, 27],
            backgroundColor: '#26C975',
            borderColor: '#26C975',
            borderWidth: 0,
            borderRadius: 6,
            borderSkipped: false,
        },
        {
            label: 'Измененных элементов',
            data: [33, 13, 22, 22, 43, 13, 13],
            backgroundColor: '#EFB000',
            borderColor: '#EFB000',
            borderWidth: 0,
            borderRadius: 6,
            borderSkipped: false,
        },
        {
            label: 'Удаленных элементов',
            data: [32, 13, 13, 33, 52, 13, 13],
            backgroundColor: '#FF6170',
            borderColor: '#FF6170',
            borderWidth: 0,
            borderRadius: 6,
            borderSkipped: false,
        }
    ]
}

/* функция для получения настроек в зависимости от размера экрана */
const getChartOptions = (isMobile = false) => {
    const baseOptions = {
        responsive: true,
        maintainAspectRatio: false,
        plugins: {
            legend: {
                display: false
            }
        },
        scales: {
            x: {
                grid: {
                    color: '#E2E2E2',
                    drawBorder: false
                },
                ticks: {
                    color: '#ADADAD',
                    font: {
                        size: 12
                    }
                }
            },
            y: {
                beginAtZero: true,
                max: 120,
                grid: {
                    color: '#E2E2E2',
                    drawBorder: false
                },
                ticks: {
                    stepSize: 20,
                    color: '#ADADAD',
                    font: {
                        size: 12
                    }
                }
            }
        }
    }

    if (isMobile) {
        // горизонтальная диаграмма для мобильных
        return {
            ...baseOptions,
            indexAxis: 'y',
            scales: {
                x: {
                    ...baseOptions.scales.x,
                    title: {
                        display: true,
                        text: 'Часы',
                        color: '#ADADAD',
                        font: {
                            size: 12
                        }
                    }
                },
                y: {
                    ...baseOptions.scales.y,
                    title: {
                        display: false
                    }
                }
            }
        }
    } else {
        // вертикальная диаграмма для десктопа
        return {
            ...baseOptions,
            scales: {
                ...baseOptions.scales,
                x: {
                    ...baseOptions.scales.x,
                    title: {
                        display: false
                    }
                },
                y: {
                    ...baseOptions.scales.y,
                    title: {
                        display: true,
                        text: 'Часы',
                        color: '#ADADAD',
                        font: {
                            size: 12
                        }
                    }
                }
            }
        }
    }
}

let chart = null

/* функция для обновления диаграммы */
const updateChart = () => {
    if (chart) {
        const isMobile = window.innerWidth < 960 // ниже планшета
        const newOptions = getChartOptions(isMobile)
        
        chart.options = newOptions
        chart.update('none') // отмена анимации для плавности
    }
}

/* обработчик изменения размера окна */
const handleResize = () => {
    updateChart()
}

onMounted(async () => {
    await nextTick()
    
    // создание диаграммы
    if (chartRef.value) {
        const ctx = chartRef.value.getContext('2d')
        const isMobile = window.innerWidth < 960
        const options = getChartOptions(isMobile)
        
        chart = new Chart(ctx, {
            type: 'bar',
            data: chartData,
            options: options
        })
        
        // добавление обработчика изменения окна
        window.addEventListener('resize', handleResize)
    }
})

onUnmounted(() => {
    // удаление обработчика при размонтировании
    window.removeEventListener('resize', handleResize)
    
    // удаление диаграммы
    if (chart) {
        chart.destroy()
    }
})

</script>