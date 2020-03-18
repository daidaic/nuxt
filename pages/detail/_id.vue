<template>
    <div>
        <h2>详情页面</h2>
        {{$route.params.id}}
        <br />
        {{title.price}}
        <br />
        {{title.description}}
    </div>
</template>
<script>

import  axios from 'axios'
export default {
//    asyncData () {
//     return axios.get('/data/test.json')
//       .then((res) => {
//         //   console.log(res)
//         return { 
//             title: res.data 
//             }
//       })
//   }
async asyncData ({ }) {
    const { data:title } = await axios.get(`/data/test.json`)
    // console.log(title)
    return { title: title}
  }
}
</script>
<style lang="sass" scoped>

</style>

