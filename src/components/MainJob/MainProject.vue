<template>
    <div class="flex space-x-4">
        <!-- In Planning Card -->
        <div class="w-72 bg-indigo-100 rounded-2xl p-3" @drop="drop($event, 'inPlanningCard')" @dragover.prevent>
            <p class="font-bold">In Planning</p>
            <hr class="border-neutral-300 my-3">

            <div class="rounded-2xl py-2 space-y-3" id="inPlanningCard">

                <div class="bg-white cursor-pointer rounded-2xl p-3" draggable="true"
                    @dragstart="drag($event, 'cardPlanning')" id="cardPlanning">
                    <div class="flex items-center justify-between mb-3">
                        <p class="inline-block text-gray-500">#CON22148</p>
                        <span class="px-4 text-gray-500 bg-green-100 rounded-2xl">Draft</span>
                    </div>
                    <h class="font-bold mt-1">CMS web application for Event Management Company</h>
                    <h1 class="text-gray-500 mt-2">Web, Mobile & Software Development</h1>
                    <div class="inline-block justify-between">
                        <div class="mt-3 pr-4 float-left">
                            <h class="text-sm text-gray-500">Industry vertical</h>
                            <p class="text-gray-500 pt-1 font-bold">Ecommerce</p>
                        </div>
                        <div class="mt-3 pr-4 float-left">
                            <h class="text-sm text-gray-500">Type</h>
                            <p class="text-gray-500 pt-1 font-bold">Small Job</p>
                        </div>
                        <div class="mt-3 pr-4 float-left">
                            <h class="text-sm text-gray-500">Requirements count</h>
                            <p class="text-gray-500 pt-1 font-bold">1</p>
                        </div>
                    </div>
                    <div class="flex items-center justify-between pt-3">
                        <div>
                            <p class="inline-block text-gray-500 text-sm">Published Date</p>
                            <p class="text-gray-500 font-bold">2024-05-28</p>
                        </div>
                        <div class="ml-auto text-right">
                            <p class="text-gray-500 text-sm">Start Date</p>
                            <p class="text-gray-500 font-bold">2024-05-28</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- In Execution Card -->
        <div class="w-72 bg-indigo-100 rounded-2xl p-3" @drop="drop($event, 'inExecutionCard')" @dragover.prevent>
            <p class="font-bold">In Execution</p>

            <hr class="border-neutral-300 my-3">

            <div class="rounded-2xl py-2 space-y-3" id="inExecutionCard">
                <div class="bg-white cursor-pointer rounded-2xl p-3 relative" draggable="true"
                    @dragstart="drag($event, 'cardExecution')" id="cardExecution">

                    <div class="absolute top-0 left-0 w-full h-2 bg-green-600 rounded-t-2xl"></div>

                    <div class="flex pt-1 items-center justify-between mb-3">
                        <p class="inline-block text-gray-500">#CON22148</p>
                        <span class="px-4 font-bold text-green-600 bg-green-200 rounded-2xl">Active</span>
                    </div>
                    <h class="font-bold mt-1">Android App Development</h>
                    <h1 class="text-gray-500 mt-2">Web, Mobile & Software Development</h1>
                    <div class="inline-block justify-between">
                        <div class="mt-3 pr-4 float-left">
                            <h class="text-sm text-gray-500">Industry vertical</h>
                            <p class="text-gray-500 pt-1 font-bold">Ecommerce</p>
                        </div>
                        <div class="mt-3 pr-4 float-left">
                            <h class="text-sm text-gray-500">Type</h>
                            <p class="text-gray-500 pt-1 font-bold">Small Job</p>
                        </div>
                        <div class="mt-3 pr-4 float-left">
                            <h class="text-sm text-gray-500">Requirements count</h>
                            <p class="text-gray-500 pt-1 font-bold">1</p>
                        </div>
                    </div>
                    <div class="flex items-center justify-between pt-3">
                        <div>
                            <p class="inline-block text-gray-500 text-sm">Published Date</p>
                            <p class="text-gray-500 font-bold">2024-05-28</p>
                        </div>
                        <div class="ml-auto text-right">
                            <p class="text-gray-500 text-sm">Start Date</p>
                            <p class="text-gray-500 font-bold">2024-05-28</p>
                        </div>
                    </div>
                </div>
            </div>

            <div class="rounded-2xl py-2 space-y-3" id="cardExecutionOverdue">

                <div class="bg-white cursor-pointer rounded-2xl p-3 relative" draggable="true"
                    @dragstart="drag($event, 'cardExecutionOverdue')" id="cardExecutionOverdue">

                    <div class="absolute top-0 left-0 w-full h-2 bg-yellow-600 rounded-t-2xl"></div>

                    <div class="flex pt-1 items-center justify-between mb-3">
                        <p class="inline-block text-gray-500">#CON22148</p>
                        <span class="px-4 font-bold text-amber-500 bg-amber-100 rounded-2xl">Overdue</span>
                    </div>
                    <h class="font-bold mt-1">Android App Development</h>
                    <h1 class="text-gray-500 mt-2">Web, Mobile & Software Development</h1>
                    <div class="inline-block justify-between">
                        <div class="mt-3 pr-4 float-left">
                            <h class="text-sm text-gray-500">Industry vertical</h>
                            <p class="text-gray-500 pt-1 font-bold">Ecommerce</p>
                        </div>
                        <div class="mt-3 pr-4 float-left">
                            <h class="text-sm text-gray-500">Type</h>
                            <p class="text-gray-500 pt-1 font-bold">Small Job</p>
                        </div>
                        <div class="mt-3 pr-4 float-left">
                            <h class="text-sm text-gray-500">Requirements count</h>
                            <p class="text-gray-500 pt-1 font-bold">1</p>
                        </div>
                    </div>
                    <div class="flex items-center justify-between pt-3">
                        <div>
                            <p class="inline-block text-gray-500 text-sm">Published Date</p>
                            <p class="text-gray-500 font-bold">2024-05-28</p>
                        </div>
                        <div class="ml-auto text-right">
                            <p class="text-gray-500 text-sm">Start Date</p>
                            <p class="text-gray-500 font-bold">2024-05-28</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Completed Card -->
        <div class="w-72 bg-indigo-100 rounded-2xl p-3 relative" @drop="drop($event, 'completedCard')"
            @dragover.prevent>
            <p class="font-bold">Completed</p>
            <hr class="border-neutral-300 my-3">

            <div class="rounded-2xl py-2 space-y-3" id="completedCard">

                <div class="bg-white cursor-pointer rounded-2xl p-3 relative" draggable="true"
                    @dragstart="drag($event, 'cardCompleted')" id="cardCompleted">
                    <div class="absolute top-0 left-0 w-full h-2 bg-green-600 rounded-t-2xl"></div>

                    <div class="flex pt-1 items-center justify-between mb-3">
                        <p class="inline-block text-gray-500">#CON22148</p>
                        <span class="px-4 font-bold text-green-600 bg-green-200 rounded-2xl">Active</span>
                    </div>
                    <h class="font-bold mt-1">Web App Development</h>
                    <h1 class="text-gray-500 mt-2">Web, Mobile & Software Development</h1>
                    <div class="inline-block justify-between">
                        <div class="mt-3 pr-4 float-left">
                            <h class="text-sm text-gray-500">Industry vertical</h>
                            <p class="text-gray-500 pt-1 font-bold">Ecommorce</p>
                        </div>
                        <div class="mt-3 pr-4 float-left">
                            <h class="text-sm text-gray-500">Type</h>
                            <p class="text-gray-500 pt-1 font-bold">Small Job</p>
                        </div>
                        <div class="mt-3 pr-4 float-left">
                            <h class="text-sm text-gray-500">Requirements count</h>
                            <p class="text-gray-500 pt-1 font-bold">1</p>
                        </div>
                    </div>
                    <div class="flex items-center justify-between pt-3">
                        <div>
                            <p class="inline-block text-gray-500 text-sm">Published Date</p>
                            <p class="text-gray-500 font-bold">2024-05-28</p>
                        </div>
                        <div class="ml-auto text-right">
                            <p class="text-gray-500 text-sm">Start Date</p>
                            <p class="text-gray-500 font-bold">2024-05-28</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    methods: {
        drag(event, cardId) {
            event.dataTransfer.setData("text", cardId);
        },
        drop(event, dropTargetId) {
            const cardId = event.dataTransfer.getData("text");
            const draggedElement = document.getElementById(cardId);
            const dropZone = document.getElementById(dropTargetId);

            if (dropZone && draggedElement) {
                if (!dropZone.contains(draggedElement)) {
                    dropZone.appendChild(draggedElement);
                }
            }
        },
    },
};
</script>

<style scoped>
.space-y-3>*+* {
    margin-top: 12px;
}
</style>
