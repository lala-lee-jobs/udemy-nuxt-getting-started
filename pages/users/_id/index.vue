<template>
  <div>
    Display your id：{{ $route.params.id }}
  </div>
</template>
<script>
export default {
  validate({params}) {
    // Must be a number 路由參數ID只能輸入數字
    // 若不為數字則會自動加載顯示404錯誤頁面
    return /^\d+$/.test(params.id);
  },
};
</script>
