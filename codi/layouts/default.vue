<template>
  <v-app>
    <v-main>
      <nuxt/>
    </v-main>
   </v-app>
</template>

<script>
export default{
  created(){
    console.log("S'ha creat el layout")
  },
  mounted(){
    console.log("S'ha muntat el layout")
  }
}
</script>