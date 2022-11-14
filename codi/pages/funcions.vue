<template>
    <div>
        Hola
    </div>
</template>
<script>
// definicio funcio suma amb es5
function suma(a,b){
    return a+b
}
// us de la funcio
console.log("Suma amb es5",suma(10,20))

// definicio de la funcio amb es6
var sumaES6 = (a,b)=>{
    return a+b
}
console.log("Suma amb es6",sumaES6(2,3))

var sumaES6_2 = (a,b)=>a+b 
let edat = 15
</script>