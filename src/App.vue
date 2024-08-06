<template>
  <div>
    <HelloWorld 
      @update-name="name => display(name)"
    />

    <!-- <span> {{ sentence }}</span>
    <br>
    <br>

    <input type="text" v-model="name"><br><br>
    <input type="number" v-model="age"> -->
  </div>

</template>

<script setup>
import HelloWorld from './components/HelloWorld.vue';

const display = (name) => {
  console.log('App.vue : ' + name)
}

// import { watch, computed, ref } from 'vue';

// const sentence = computed(() => {
//   return `Bonjour, je m'appelle ${name.value} et j'ai ${age.value} ans.`
// })
// const name = ref('Bideew')
// const age = ref(24)

// watch (name, (newValue, oldValue) => {
//   console.log(newValue, oldValue)
// })


// const user = reactive({
//   name: "Bideew ",
//   age: 24,
// })
// const display = () => {
//   console.log(user.name, user.age)
// }
// display()

</script>

<style scoped>
.bold {
  font-weight: bolder;
}

.text-red {
  color: indianred;
  font-size: 2em;
}

.text-green {
  color: green;
  font-size: 2em;
}
</style>
