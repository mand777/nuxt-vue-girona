<template>
    <div>

    </div>
</template>

<script>
console.log('abans del fetch')
fetch('https://dummyjson.com/users')
.then(res =>{
    console.log('primer then')
   return  res.json()
} )
.then((usuaris)=>{
    console.log("segon then")
    console.log(usuaris)
});
console.log('despres del fetch')

fetch('https://dummyjson.com/users/1')
.then(res => res.json())
.then(console.log);


</script>