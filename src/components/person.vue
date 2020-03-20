<template>
    <div>
        姓名：{{person.name}}
        年龄：{{person.age}}
        性别：{{person.gender}}
    </div>
</template>

<script>
    export default {
        name: "person.vue",
        props: {
            person: {
                type: Object
            }
        }
    }
</script>

<style scoped>

</style>
