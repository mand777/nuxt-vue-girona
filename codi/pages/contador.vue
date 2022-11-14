<template>
    <div>
        <h1>{{titol}}</h1>
        <p v-html="descripcio"></p>
        {{contador}}
        <button v-on:click="augmentar()">augmentar</button>
        <button @click="disminuir()">disminuir</button>
    </div>
</template>

<script>
    export default {
        data:function(){
            return{
                titol:"Contador vue",
                descripcio:"El contador <strong>del</strong> curs vue girona",
                contador:0
            }
        },
        methods:{
            augmentar:function(){
                this.contador++
                this.titol = "He augmentat"
            },
            disminuir:function(){
                this.contador--
                this.titol = "He disminuit"
            }
        }
    }
</script>