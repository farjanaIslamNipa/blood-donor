<template>
    <div>
        <div class="bg-white min-h-screen flex items-center text-lg">
            <form action="" class="p-10 md:w-2/3 lg:w-1/2 mx-auto rounded">
                <div class="shadow">
                    <div class="flex items-center bg-gray-200 rounded-t-lg mb-5">
                        <label for="name" class="w-40 text-right mr-8 p-4 text-gray-800 text-[15px]">Donar Name</label>
                        <input v-model.trim="donarName.val" type="text" name="name" id="name" placeholder="Put in your name"
                            class="flex-1 p-4 pl-0 bg-transparent placeholder-gray-400 placeholder:text-[15px]  outline-none text-white overflow-ellipsis overflow-hidden">
                    </div>
                    <p v-if="donarName.isValid" class="text-red-700">Please input your name!!</p>
                    <div class="flex items-center bg-gray-200 mb-5">
                        <label for="twitter" class="w-40 text-right p-4 mr-8 text-gray-800 text-[15px]">Donar Age</label>
                        <input v-model.trim="donarAge.val" type="text" name="twitter" id="age"
                            placeholder="Put your age here"
                            class="flex-1 p-4 pl-0 bg-transparent placeholder-gray-400 placeholder:text-[15px] outline-none text-white overflow-ellipsis overflow-hidden">
                    </div>

                    <p v-if="donarName.isValid" class="text-red-700">Please input your Blood Group!!</p>
                    <div class="flex items-center bg-gray-200 mb-5">
                        <label for="twitter" class="w-40 text-right p-4 mr-8 text-gray-800 text-[15px]">Blood Group</label>
                        <input v-model.trim="bloodGroup.val" type="text" name="twitter" id="age"
                            placeholder="Put your Blood Group"
                            class="flex-1 p-4 pl-0 bg-transparent placeholder-gray-400 placeholder:text-[15px] outline-none text-white overflow-ellipsis overflow-hidden">
                    </div>

                    <p v-if="donarAge.isValid" class="text-red-700">Please input your age!!</p>
                    <div class="flex items-center bg-gray-200 mb-5">
                        <label for="twitter" class="w-40 text-right p-4 mr-8 text-gray-800 text-[15px]">Donar phone</label>
                        <input v-model="donarPhone.val" type="number" name="twitter" id="phone"
                            placeholder="Put your phone number here"
                            class="flex-1 p-4 pl-0 bg-transparent placeholder-gray-400 placeholder:text-[15px] outline-none text-white overflow-ellipsis overflow-hidden">
                    </div>
                    <p v-if="donarPhone.isValid" class="text-red-700">Please input your phone!!</p>
                    <div class="flex items-center bg-gray-200 mb-5">
                        <label for="twitter" class="w-40 text-right p-4 mr-8 text-gray-800 text-[15px]">Donar Info</label>
                        <input v-model="donarInfo.val" type="text" name="twitter" id="info"
                            placeholder="Put your information here"
                            class="flex-1 p-4 pl-0 bg-transparent placeholder-gray-400 placeholder:text-[15px] outline-none text-white overflow-ellipsis overflow-hidden">
                    </div>
                    <p v-if="donarId.isValid" class="text-red-700">Please input your Id!!</p>
                    <div class="flex items-center bg-gray-200 mb-5">
                        <label for="twitter" class="w-40 text-right p-4 mr-8 text-gray-800 text-[15px]">Donar Id</label>
                        <input v-model="donarId.val" type="text" name="twitter" id="id" placeholder="Put your age here"
                            class="flex-1 p-4 pl-0 bg-transparent placeholder-gray-400 placeholder:text-[15px] outline-none text-white overflow-ellipsis overflow-hidden">
                    </div>
                    <p v-if="totalDotation.isValid" class="text-red-700">Please input your Total Donate Time!!</p>
                    <div class="flex items-center bg-gray-200 mb-5">
                        <label for="twitter" class="w-40 text-right p-4 mr-8 text-gray-800 text-[15px]">Total Donate Time</label>
                        <input v-model="totalDotation.val" type="text" name="twitter" id="time"
                            placeholder="Put your age here"
                            class="flex-1 p-4 pl-0 bg-transparent placeholder-gray-400 placeholder:text-[15px] outline-none text-white overflow-ellipsis overflow-hidden">
                    </div>
                </div>
                <button class="bg-red-700 block w-full rounded py-4 text-white font-bold shadow rounded-t-none rounded-b-lg">Submit</button>

            </form>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue';

const donarName = ref({
    val: '',
    isValid: false,
})
const donarAge = ref({
    val: '',
    isValid: false,
})
const donarInfo = ref({
    val: '',
    isValid: false,
})
const donarId = ref({
    val: '',
    isValid: false,
})
const donarPhone = ref({
    val: '',
    isValid: false,
})
const totalDotation = ref({
    val: '',
    isValid: false,
})
const bloodGroup = ref({
    val: '',
    isValid: false,
})
const formIsValid = ref(true)

</script>
