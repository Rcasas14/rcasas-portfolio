<template>
    <div class="nav-wrapper border-b-[1px]">
    <nav class="min-h-[76px] mx-[30px] ">
        <ul class="flex justify-between items-center">
            <li class=""><a href="#">Reymart Casas.</a></li>
            <li class="flex-1 mx-10">
                <a href="#" class="navlinks m-5">Home</a>
                <a href="#" class="navlinks m-5">Projects</a>
            </li>
            <li class="flex items-center">
                <a href="#" class="navlinks m-5">Github</a>
                <a href="" class="navlinks m-5"><img src="../assets/dark-mode-icon.svg" alt=""></a>
            </li>
        </ul>
    </nav>
</div>
</template>

<script>
export default{
    props: ['navItems', 'activeNavItem'],
    data(){
        return {
        }
    }   
}

</script>