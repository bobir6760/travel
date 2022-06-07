<template>
  <div class="globally-item">
    <div class="globally-item__title">For Domestic</div>
    <button class="globally-btn">Start trip today</button>
  </div>
</template>

<script>
export default {
  name: "global-card",
};
</script>

<style scoped lang="scss">
.globally-btn {
  padding: 12px 30px;
  border-radius: 30px;
  background: none;
  color: white;
  border-color: white;
  cursor: pointer;
  font-size: 12px;
}
.globally-btn:active {
  color: white;
  background: #571d1d;
}
.globally-item__title {
  font-size: 15px;
  color: white;
  font-weight: bold;
}
</style>
