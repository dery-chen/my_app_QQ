<template>
   <div class="list">
    <dl v-for="item in dataList" :key="item.id">
      <dt><img src="http://dummyimage.com/50x50" alt=""></dt>
      <dd>
        <p>{{item.name}}</p>
        <p>{{item.msg}}</p>
      </dd>
    </dl>
    </div>
</template>

<script>
export default {
 props:["dataList"]
}
</script>

<style>

</style>