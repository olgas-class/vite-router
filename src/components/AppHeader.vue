<script>
export default {
    data() {
        return {
            menu: [
                {
                    title: "Home",
                    routeName: "home",
                },
                {
                    title: "About",
                    routeName: "about",
                }
            ]
        }
    }

}
</script>

<template>
    <header>
        <ul>
            <li v-for="item in menu"> 
                <router-link :to="{name: item.routeName}" >
                    {{ item.title }}
                </router-link>
             </li>
        </ul>
    </header>
</template>

<style scoped lang="scss">
</style>