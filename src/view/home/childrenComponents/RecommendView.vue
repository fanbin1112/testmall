<template>
  <div class="recommend">
    <div v-for="(item,index) in recommends" :key="index" class="recommend-item">
      <a :href="item.link">
        <img :src="item.image" alt />
        <div>{{item.title}}</div>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "RecommendView",
  data() {
    return {};
  },
  props: {
    recommends: {
      type: Array,
      default() {
        return [];
      },
    },
  },
};
</script>

<style scoped>
  .recommend {
    display: flex;
    width: 100%;
    text-align: center;
    font-size: 12px;
    padding: 15px 0 20px;
    border-bottom: 8px solid #eee;
    
  }
  .recommend-item {
    flex: 1;
  }
  .recommend-item a {
    text-decoration: none;
    color: grey;
  }
  .recommend-item img {
    width: 70px;
    height: 70px;
    margin-left: 13px;
    margin-bottom: 10px;
  }
  
</style>
