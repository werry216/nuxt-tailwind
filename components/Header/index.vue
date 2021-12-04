<template>
    <div class="bg-white shadow border-t-4 h-16 border-blue-300 rounded-b-lg fixed w-full top-0">
        <div class="container mx-auto px-4">
            <div class="hidden sm:flex items-center justify-end py-4">
                <div class="hidden sm:flex sm:items-center">
                    <a href="#" class="text-green-500 text-sm font-semibold mr-4">Login</a>
                </div>
            </div>
            // Here is the main content...
            <div class="block sm:hidden bg-white py-2">
                <div class="flex flex-col">
                    <div class="flex justify-end items-center pt-2">
                        <a
                            href="#"
                            class="text-gray-800 text-sm font-semibold hover:text-purple-600 mr-4"
                        >Login</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    components: {
    },
}
</script>
