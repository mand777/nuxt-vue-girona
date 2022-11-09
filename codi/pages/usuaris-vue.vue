<template>
    <div>
        <button v-on:click="descarregarUsuaris()">descarregar</button>
        <button v-on:click="descarregarUsuaris2()">async descarregar</button>
        <pre>
            {{usuaris}}
        </pre>
    </div>
</template>

<script>
export default{
    data:function(){
        return{
            usuaris:[]
        }

    },
    methods:{
        descarregarUsuaris(){
           var f= fetch("https://dummyjson.com/users")

           var j= f.then(function(resposta){
            return resposta.json()
           })

           var self=this

           j.then(function(dades){
            console.log(dades)
            self.usuaris=dades
           })


        },
        async descarregarUsuaris2(){
            var resposta= await fetch("https://dummyjson.com/users")
            //console.log(resposta)

            var dades= await resposta.json()
            console.log(dades)

        }

    }
}
</script>