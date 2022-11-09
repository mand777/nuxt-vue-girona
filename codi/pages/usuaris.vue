<template>
    <div>

    </div>
</template>
<script>

fetch("https://dummyjson.com/users")
.then(res=>{
    return res.json()
})
.then((usuaris)=>{
    console.log(usuaris)
});

console.log("despres del fetch")

fetch("https://dummyjson.com/users/1")
.then(res.json())
.then(console.log);

</script>
