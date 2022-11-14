<template>
    <div>
        porfoli
        <Hola></Hola>
    </div>
</template>
<script>

 import Hola from '../prova/Hola.vue'

 var usuaris = []

 export default{
    components:{
         Hola:Hola,
    },
    layout:"basic"
}
</script>