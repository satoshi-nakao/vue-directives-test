<template>
  <div>
  <h1>{{ message }}</h1>
    <p>ulタグを場合</p>
    <ul>
      <li v-for="num in numbers" :key="num">{{ num }}</li>
    </ul>
    <p>olタグを場合</p>
    <ol>
      <li v-for="boy in boys" :key="boy">{{ boy }}</li>
    </ol>
  </div>
</template>

<script>


export default {
  data: function() {
    return {
      message: "v-forを使った条件付きレンダリングのテスト",
      numbers :[1,2,3,4,5,6,7,8,9,10],
      boys : ["太郎","博","孝介","昭雄"]
    }
  }
}
</script>


