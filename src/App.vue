<template>
  <n-scrollbar x-scrollable>
  <div class="container" style="height:400px;width:800px;background-color:#fff;contain: layout paint;">
    <n-config-provider style="height: 100%">
      <n-modal :show="true" to="container">
        <n-card
          content-style="padding: 0;"
          style="width: 200px; height: 50px; text-align: center; line-height: 50px"
          size="huge"
          :bordered="false"
          role="dialog"
          aria-modal="true"
        >加载中……</n-card>
      </n-modal>
      <div class="container" id="mysql-container" ref="loadingBarTargetRef">
        <n-layout has-sider style="height: 100%">
          <n-layout-sider class="n-layout-sider-style-width" :width="180">
            <div class="side-box">
              <div>
                <div>111111</div>
                <div>222222</div>
              </div>
            </div>
          </n-layout-sider>
          <n-layout style="height: 100%">
            <n-layout-content style="height: 100%">
              <div class="content-flex">
                <div>111111</div>
                <div>222222</div>
              </div>
            </n-layout-content>
          </n-layout>
        </n-layout>
      </div>
    </n-config-provider>
  </div>
  </n-scrollbar>
</template>
<script lang="ts" setup>

</script>
<style scoped>
.container {
  height: 100%;
}
.side-box {
  height: 100%;
  padding: 10px 0 0 10px;
  box-sizing: border-box;
}
.content-flex{
  display: flex;
  justify-content: space-between;
  background-color: #ff0000;
}
.n-layout-sider-style-width{
  height: 100%;
}
.tips-text {
  color: #ff0000;
  font-size: 12px;
  padding: 20px 0 0 0;
}
</style>
