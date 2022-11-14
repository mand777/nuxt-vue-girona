<template>
    <div>
        <div>{{contador}}</div>
        <v-btn v-on:click="augmentar10()" >augmentar 10</v-btn>
        <v-btn @click="disminuir10()">disminuir 10</v-btn>
    </div>
</template>

<script>
export default {
    data:function(){
        return{
            contador:0
        }
    },
    methods:{
        augmentar10:function(){
            this.contador += 10
        },
        disminuir10(){
            this.contador -= 10
        }
    }
}
</script>