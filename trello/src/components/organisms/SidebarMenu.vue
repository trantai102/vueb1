<template>
    <n-space vertical size="large">
        <n-layout has-sider>
            <n-layout-sider collapse-mode="width" :collapsed-width="96" :native-scrollbar="true" :width="240"
                show-trigger="arrow-circle" content-style="padding: 24px;" bordered>
                <a class="text-2xl font-bold text-center mb-10 block" href="/">Trello</a>
                <n-menu :collapsed-width="64" :collapsed-icon-size="22" :options="menuOptions" >
                </n-menu>
            </n-layout-sider>
        </n-layout>
    </n-space>
</template>
<script>
import { h, defineComponent } from "vue";
import { NIcon } from "naive-ui";
import {
    SearchOutline as SearchIcon,
    HomeOutline as HomeIcon,
    CardOutline as CardIcon,
    SettingsOutline as SettingsIcon,
    
} from "@vicons/ionicons5";

function renderIcon(icon) {
    return () => h(NIcon, null, { default: () => h(icon) });
}

const menuOptions = [
    {
        label: "Search",
        key: "1",
        icon: renderIcon(SearchIcon),
    },
    {
        label: "Home",
        key: "2",
        icon: renderIcon(HomeIcon),
    },
    {
        label: "Card",
        key: "3",
        icon: renderIcon(CardIcon)
    },
    {
        label: "Setting",
        key: "4",
        icon: renderIcon(SettingsIcon),
       
    }
];

export default defineComponent({
    setup() {
        return {
            menuOptions
        };
    }
});
</script>
<style lang="">

</style>