<template>
    <h1>Retndering List Data</h1>
    <ul>
        <li v-for="person in listOfPersons" :key="person">Name: {{person.name}} , Lastname: {{person.lname}}</li>
        <br>
    </ul>                               <!-- Using v-for loop to show the list data -->
</template>
<script>
export default {
    name:'renderinglist',
    data(){
        return{
            listOfPersons:[{name:'Tony',lname:'Stark'},{name:'Bruce',lname:'Banner'}] // array list with objects
        }
    }
}
</script>