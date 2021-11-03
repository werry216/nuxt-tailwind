<template>
    <div class="mb-24 w-full p-4 flex flex-col justify-center items-center">
        <div class="flex flex-wrap w-full">
            <div class="w-full">
                <ul class="flex mb-0 list-none flex-wrap pt-3 pb-4 flex-row">
                    <li class="-mb-px last:mr-0 text-center w-1/3">
                        <a
                            class="cursor-pointer text-xs uppercase px-5 py-3 shadow-lg rounded block leading-normal"
                            v-on:click="toggleTabs(1)"
                            v-bind:class="{ 'text-green-300 bg-white': openTab !== 1, 'text-white bg-green-300': openTab === 1 }"
                        >Arbeitnehmer</a>
                    </li>
                    <li class="-mb-px last:mr-0 text-center w-1/3">
                        <a
                            class="cursor-pointer text-xs uppercase px-5 py-3 shadow-lg rounded block leading-normal"
                            v-on:click="toggleTabs(2)"
                            v-bind:class="{ 'text-green-300 bg-white': openTab !== 2, 'text-white bg-green-300': openTab === 2 }"
                        >Arbeitgeber</a>
                    </li>
                    <li class="-mb-px last:mr-0 text-center w-1/3">
                        <a
                            class="cursor-pointer text-xs uppercase p-3 text-center shadow-lg rounded block leading-normal"
                            v-on:click="toggleTabs(3)"
                            v-bind:class="{ 'text-green-300 bg-white': openTab !== 3, 'text-white bg-green-300': openTab === 3 }"
                        >Temporärbüro</a>
                    </li>
                </ul>
                <div
                    class="flex flex-col min-w-0 break-words bg-white w-full mb-6 shadow-lg rounded"
                >
                    <div class="px-4 py-5 flex-auto">
                        <div class="tab-content tab-space">
                            <div v-bind:class="{ 'hidden': openTab !== 1, 'block': openTab === 1 }">
                                <Page1></Page1>
                            </div>
                            <div v-bind:class="{ 'hidden': openTab !== 2, 'block': openTab === 2 }">
                                <Page2></Page2>
                            </div>
                            <div v-bind:class="{ 'hidden': openTab !== 3, 'block': openTab === 3 }">
                                <Page3></Page3>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import Page1 from "~/components/Content/page1";
import Page2 from "~/components/Content/page2";
import Page3 from "~/components/Content/page3";

export default {
    components: {
        Page1,
        Page2,
        Page3,
    },
    data() {
        return {
            openTab: 1
        }
    },
    methods: {
        toggleTabs: function (tabNumber) {
            this.openTab = tabNumber
        }
    }
}
</script>
