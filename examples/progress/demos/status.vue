<template>
  <div>
    <div>
      <div >进度完成：</div>
      <t-progress class="t-progress-domo-margin" theme="line" :status="'success'" :percentage="80" ></t-progress>
      <t-progress class="t-progress-domo-margin" theme="plump" :status="'success'" :percentage="80" ></t-progress>
      <t-progress class="t-progress-domo-margin" theme="circle" :status="'warning'" :percentage="80" ></t-progress>
    </div>
    <div>
      <div >进度状态出现重大错误（如下载的文件有损）：</div>
      <t-progress class="t-progress-domo-margin" theme="line" :status="'error'" :percentage="80" ></t-progress>
      <t-progress class="t-progress-domo-margin" theme="plump" :status="'error'" :percentage="80" ></t-progress>
      <t-progress class="t-progress-domo-margin" theme="circle" :status="'error'" :percentage="80" ></t-progress>
    </div>
    <div>
      <div >进度被中断（如失去网络连接）</div>
      <t-progress class="t-progress-domo-margin" theme="line" :status="'warning'" :percentage="80" ></t-progress>
      <t-progress class="t-progress-domo-margin" theme="plump" :status="'warning'" :percentage="80" ></t-progress>
      <t-progress class="t-progress-domo-margin" :percentage="80" :status="'warning'"></t-progress>
      <t-progress class="t-progress-domo-margin" theme="circle" :status="'warning'" :percentage="80" ></t-progress>
    </div>
  </div>
</template>
<style scoped>
.t-progress-domo-margin{
  margin: 20px 0 10px
}
</style>
