<template>
  <div class="home">
    <van-cell-group>
      <van-field v-model="value" placeholder="请输入商品名称" />
    </van-cell-group>
    <van-cell-group>
      <van-field v-model="value" placeholder="请输入商品价格" />
    </van-cell-group>
    <van-cell-group>
      <van-field v-model="value" placeholder="请输入商品数量" />
    </van-cell-group>
    <van-button type="primary">添加商品</van-button>
    <van-card
      price="2.00"
      title="商品标题"
    >
      <div slot="footer">
        <van-button size="mini">按钮</van-button>
        <van-button size="mini">按钮</van-button>
      </div>
    </van-card>
    <van-submit-bar :price="3050" button-text="提交订单" @submit="onSubmit">
      <van-checkbox v-model="checked">全选</van-checkbox>
      <van-button type="primary">批量删除</van-button>
    </van-submit-bar>
  </div>
</template>

<script>
export default {
  data() {
    return {
      value: ""
    };
  }
};
</script>
