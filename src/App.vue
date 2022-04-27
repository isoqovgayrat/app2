<template>
  <div>
  <span v-text="msg">
  </span>
    <span v-html="title"></span>
  </div>
  <div v-if="isAdmin">
   <h1> Assalomu alaykum, xurmatli adminstrator!</h1>
  </div>
  <div v-else="isAdmin">
    <h1> Assalomu alaykum, xurmatli foydalanuvchi!</h1>
  </div>
  <div>
    <p v-if="word === 'car'">Mashina</p>
    <p v-else-if="word === 'animal'">Hayvon</p>
    <p v-else-if="word === 'book'">Kitob</p>
    <p v-else>Bunday so'z mavjud emas!</p>
  </div>
  <div v-show="isBool">
    <h1>Men ko'rinyapman!</h1>
  </div>
  <div>
<!--    <p v-for="i in 10">{{i}}</p>-->
    <p v-for="i in 10">Salom</p>
  </div>
</template>

<script>


export default {
  name: 'App',
  data() {
    return {
      msg: "Biror xabar",
      title: "<h1>Salom Dunyo</h1>",
      isAdmin: false,
      word: "kwenkdnwekd",
      isBool:true,
    }
  }

}
</script>

<style>

</style>
