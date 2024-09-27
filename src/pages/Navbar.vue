<template>
    <div class="bg-white rounded-2xl p-3 fixed w-max width ml-36">
        <div class="flex items-start space-x-6">
            <div class="flex items-center p-2 space-x-4">
                <span class="material-icons">search</span>
                <!-- <AutoInput class="w-full border-none" :placeholder="'Search'"></AutoInput> -->
                <input type="text" placeholder="Search" class="rounded-lg py-2 focus:outline-none focus:ring-0" />
            </div>

            <div class="bg-fuchsia-200 p-2 rounded-2xl flex items-center space-x-2">
                <span class="material-icons">error</span>
                <p class="text-fuchsia-950 font-semibold">Complete your profile</p>
                <a href="#" class="flex hover:bg-fuchsia-200 items-center text-black py-2.5 pr-4 rounded">
                    <span class="ml-2"><u><b>Let's Go</b></u></span>
                </a>
            </div>


            <div class="bg-slate-100 flex rounded-2xl items-center space-x-2 rounded-lg p-4">
                <span class="material-icons">error</span>
                <p><b>Board</b></p>
            </div>

            <div class="bg-slate-100 flex items-center rounded-lg p-4">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path
                        d="M11.5119 2.99609C13.2885 2.99622 14.9923 3.70203 16.2486 4.9583C17.5048 6.21456 18.2107 7.91838 18.2108 9.695V17.4144H4.8125V9.695C4.81262 7.9183 5.5185 6.2144 6.77487 4.95813C8.03123 3.70185 9.73517 2.99609 11.5119 2.99609V2.99609Z"
                        stroke="#333333" stroke-width="1.39024" stroke-linecap="round" stroke-linejoin="round" />
                    <path d="M3.09375 17.4141H19.9364" stroke="#333333" stroke-width="1.39024" stroke-linecap="round"
                        stroke-linejoin="round" />
                    <path
                        d="M14.7031 17.4141C14.7031 19.0144 13.2753 20.3114 11.5156 20.3114C9.75594 20.3114 8.32812 19.0144 8.32812 17.4141"
                        stroke="#333333" stroke-width="1.39024" stroke-linecap="round" stroke-linejoin="round" />
                </svg>
                <span class="px-2"> | </span>
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <g clip-path="url(#clip0_602_13986)">
                        <path
                            d="M12 0C5.36761 0 0 5.367 0 12C0 18.6323 5.367 24 12 24C18.6324 24 24 18.633 24 12C24 5.36761 18.633 0 12 0ZM12 22.3256C6.30647 22.3256 1.67442 17.6936 1.67442 12C1.67442 6.30642 6.30647 1.67442 12 1.67442C17.6936 1.67442 22.3256 6.30642 22.3256 12C22.3256 17.6936 17.6936 22.3256 12 22.3256Z"
                            fill="#333333" />
                        <path
                            d="M11.6458 15.1836C10.9824 15.1836 10.4453 15.7364 10.4453 16.3998C10.4453 17.0475 10.9666 17.6161 11.6458 17.6161C12.325 17.6161 12.862 17.0475 12.862 16.3998C12.862 15.7364 12.3092 15.1836 11.6458 15.1836Z"
                            fill="#333333" />
                        <path
                            d="M11.8539 5.97559C9.7215 5.97559 8.74219 7.23929 8.74219 8.09223C8.74219 8.70826 9.26344 8.9926 9.68991 8.9926C10.5429 8.9926 10.1954 7.77629 11.8065 7.77629C12.5963 7.77629 13.2282 8.12382 13.2282 8.85043C13.2282 9.70337 12.3436 10.193 11.8223 10.6353C11.3642 11.0301 10.764 11.6778 10.764 13.0362C10.764 13.8576 10.9852 14.0945 11.6328 14.0945C12.4067 14.0945 12.5647 13.747 12.5647 13.4469C12.5647 12.6255 12.5805 12.1516 13.4493 11.4724C13.8757 11.1407 15.2183 10.0666 15.2183 8.58184C15.2183 7.09707 13.8757 5.97559 11.8539 5.97559Z"
                            fill="#333333" />
                    </g>
                    <defs>
                        <clipPath id="clip0_602_13986">
                            <rect width="24" height="24" fill="white" />
                        </clipPath>
                    </defs>
                </svg> <span class="px-2">|</span>
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <g clip-path="url(#clip0_602_13998)">
                        <path
                            d="M11.131 12.207C10.576 12.75 9.849 13.021 9.122 13.021C8.39 13.021 7.658 12.746 7.102 12.196L5.322 10.436C4.929 10.048 4.926 9.415 5.314 9.022C5.702 8.629 6.334 8.626 6.728 9.014L8.508 10.774C8.844 11.106 9.392 11.109 9.732 10.777L13.3 7.285C13.695 6.898 14.327 6.907 14.714 7.301C15.1 7.696 15.093 8.329 14.698 8.715L11.131 12.207ZM24 17V21C24 22.654 22.654 24 21 24H14.621C12.721 24 11.07 22.647 10.698 20.784L10.059 17.588C9.882 16.704 10.109 15.796 10.681 15.098C11.252 14.401 12.098 14 13 14H16.183L15.603 10.735C15.546 10.401 15.574 10.216 15.596 10.136C15.784 9.446 16.346 9 17.028 9C17.241 9 17.456 9.044 17.668 9.132C17.922 9.237 18.171 9.499 18.35 9.851L20.543 14H20.999C22.653 14 24 15.346 24 17ZM14.621 22H20V16H13.001C12.7 16 12.419 16.133 12.229 16.365C12.038 16.598 11.962 16.901 12.021 17.195L12.66 20.391C12.847 21.323 13.672 21.999 14.622 21.999L14.621 22ZM7.777 17.688C4.376 16.706 2 13.544 2 10C2 5.589 5.589 2 10 2C13.06 2 15.807 3.703 17.169 6.445C17.414 6.94 18.013 7.143 18.51 6.896C19.004 6.65 19.206 6.05 18.96 5.556C17.257 2.128 13.824 0 10 0C4.486 0 0 4.486 0 10C0 14.43 2.97 18.381 7.223 19.609C7.316 19.635 7.409 19.648 7.5 19.648C7.935 19.648 8.334 19.364 8.461 18.925C8.614 18.395 8.308 17.841 7.777 17.688Z"
                            fill="#333333" />
                    </g>
                    <defs>
                        <clipPath id="clip0_602_13998">
                            <rect width="24" height="24" fill="white" />
                        </clipPath>
                    </defs>
                </svg>
            </div>

            <div class="flex flex-row pt-2 items-center">
                <div class="mr-2">
                    <img src="C:\Users\J.K.INFOTECH\Vue_Project\vue-tail-project\src\assets\author.png"
                        class="h-10 w-10 rounded-full object-cover border-outline">
                </div>
                <div class="flex flex-col">
                    <p class="pl-2 amanfont font-bold">Aman</p>
                    <p class="pl-2 text-gray-400">Customer</p>
                </div>

                <span class="bg-fuchsia-200 ml-4 h-7 w-7 flex items-center justify-center rounded-full">
                    <span class="material-icons text-fuchsia-950">keyboard_arrow_up</span>
                </span>

            </div>
        </div>
    </div>
</template>

<script>
import AutoInput from '@/components/AutoInput.vue';

export default {
    name: "Navbar",

    components: {
        AutoInput
    },

};

</script>

<style scoped>
.width {
    width: 1070px !important;
}

.amanfont {
    font-family: 'Poppins', sans-serif;
    font-weight: 500px;
    font-size: 16px;
}
</style>