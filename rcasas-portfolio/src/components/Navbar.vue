<template>
    <div class="nav-wrapper border-b-[1px]">
    <nav class="min-h-[76px] mx-[30px] ">
        <ul class="flex justify-between items-center">
            <li class=""><a href="#home">Reymart Casas.</a></li>
            <li class="flex-1 mx-10">
                <a class="navlinks m-5"
                v-for="(item, index) in navItems" :key="index"
                :class="{active: activeNavItem == index}"
                :href="item.url"
                :id="item.url"
                @click.prevent="activeNavItem = index"
                >{{ item.text }}</a>
                
            </li>
            <li class="flex items-center">
                <a href="#github" id="github" class="navlinks m-5">Github</a>
                <a href="#" class="navlinks m-5"><img src="../assets/dark-mode-icon.svg" alt=""></a>
                
            </li>
        </ul>
    </nav>
</div>
</template>

<script>
export default{
    props: {
        navItems: {
            type: Array,
            required: true
        }, 
    },
    data(){
        return {
            activeNavItem: 0,
        }
    }   
}

</script>

<style scoped>
.active {
    color: #fff;
    opacity: 0.7;
}

</style>