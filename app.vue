<template>
  <div>
    <!-- <ul>
      <li v-for="post in posts" :key="posts.id">
        {{ user.name }}
      </li>
    </ul> -->
    wewe
  </div>
</template>

<script setup>
const client = useSupabaseClient();
// const { data, error } = await useAsyncData('tests', async () => {
//   const { data } = await client.from('test').select();
//   console.log(data);
//   return data;
// });

let { data, error } = await client.from('test').select('*');

// console.log(data);
console.log(data);
console.log(error);
</script>
