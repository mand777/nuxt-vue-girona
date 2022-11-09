<template>
    <div>
        <h1>{{titol}}</h1>
        <p v-html="descripcio"></p>
       {{contador}}
       <button v-on:click="augmentar()">+</button>
       <button @click="disminuir()">-</button> 
    </div>
</template>

<script>
    export default {
        data: function(){
            return{
                titol:"contador vue",
                descripcio:"el contador <strong>del</strong> del curs vue girona",
                contador:0


            }

        },
        methods:{
            augmentar:function() {
                this.contador++
                this.titol= "he augmentat"
            },
        
            disminuir:function(){
                this.contador--
                this.titol="he disminuit"
            }
    }}
</script>