<template>
    <nav>
        <a 
        v-for="(item,index) in navItems"
        :key="index" 
        :href="item.src"
        >
        {{ item.name }}
        </a>
    </nav>
</template>

<script>
export default {
    data() {
        return {
            navItems:[
            {
                name:'Home',
                src:'#',
                isActive:true
            },
            {
                name:'About me',
                src:'#',
                isActive:false
            },
            {
                name:'My portfolio',
                src:'#',
                isActive:false
            },
            ]
        }
    },
}
</script>

<style scoped>

.navbar
{

}

</style>
