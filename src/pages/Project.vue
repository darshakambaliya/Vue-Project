<template>
    <div class="ml-36">
        <div class="flex">
            <p class="text-black pr-2">Home</p> /
            <p class="text-black pl-2"><b>Project</b></p>
        </div>
        <div class="my-10 text-xl">
            <p class="font-bold">Kanban</p>
        </div>
        <div class="bg-white rounded-2xl p-3 w-max width">
            <div class="flex items-center">
                <div class="border-2 mr-3 rounded-lg border-purple-200 py-3 px-11 cursor-pointer transition"
                    @click="selectTab('Jobs')" :class="selectedTab == 'Jobs' ? 'text-purple-950 bg-purple-200' : ''">
                    <p :class="{ 'font-bold': selectedTab === 'Jobs' }">Jobs</p>
                </div>
                <div class="border mr-3 rounded-lg border-purple-200 py-3 px-11 cursor-pointer transition"
                    @click="selectTab('Contracts')"
                    :class="selectedTab == 'Contracts' ? 'text-purple-950 bg-purple-200' : ''">
                    <p :class="{ 'font-bold': selectedTab === 'Contracts' }">Contracts</p>
                </div>
                <div class="border mr-3 rounded-lg border-purple-200 py-3 px-11 cursor-pointer transition"
                    @click="selectTab('Projects')"
                    :class="selectedTab == 'Projects' ? 'text-purple-950 bg-purple-200' : ''">
                    <p :class="{ 'font-bold': selectedTab === 'Projects' }">Projects</p>
                </div>
                <div class="flex items-center w-96 border-2 rounded-lg px-2 ml-auto">
                    <span class="material-icons">search</span>
                    <input type="text" placeholder="Search in jobs"
                        class="rounded-lg p-3 focus:outline-none focus:ring-0" />
                </div>
            </div>
        </div>

        <MainProject class="width mt-5"></MainProject>

    </div>
</template>

<script>
import MainProject from '@/components/MainJob/MainProject.vue';


export default {
    name: "Project",
    data() {
        return {
            selectedTab: 'Projects',
        };
    },

    components: {
        MainProject,
    },

    methods: {
        selectTab(tab) {
            console.log('selected tab name', this.selectedTab);
            this.selectedTab = tab;

        },
    },

};

</script>

<style scoped>
.width {
    width: 1070px !important;
}
</style>