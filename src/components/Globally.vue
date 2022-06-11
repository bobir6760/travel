<template>
  <div class="globally">
    <div class="container">
      <div class="globally-wrapper">
        <div class="globally-info">
          <div class="globally-info__title"><span>Globally</span> Accepted</div>
          <div class="globally-info__subtitle">
            Lorem Ipsum is simply dummy text of the printing and typesetting
            industry. Lorem Ipsum <br />has been the industry's standard dummy
            text ever since the 1500s, when an unknown <br />printer took a
            galley of type and scrambled it to make a type specimen book.
          </div>
        </div>
        <div class="globally-card-wrapper">
          <GlobalCard />
          <GlobalCard />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import GlobalCard from "@/components/GlobalCard";

export default {
  name: "Globally",
  components: {
    GlobalCard,
  },
};
</script>

<style lang="scss" scoped>
.globally {
  padding: 50px 0px;
  .globally-wrapper {
    display: flex;
    flex-direction: column;
    text-align: center;
    gap: 50px;
  }
}
$fz: 25px;
.globally-info {
  display: flex;
  flex-direction: column;
  gap: 30px;
}
.globally-card-wrapper {
  display: flex;
  justify-content: center;
  gap: 30px;
}
.globally-info__subtitle {
  font-size: 15px;
}
.globally-item {
  display: flex;
  flex-direction: column;
  gap: 10px;
  border-radius: 10px;
  border: none;
  padding: 50px 70px;
  background: #7f2736;
  opacity: 0.8;
}
.globally-info__title {
  font-size: $fz;
  font-weight: bold;
  cursor: pointer;
  span {
    color: #7f2736;
  }
}
@media screen and (max-width: 768px) {
  .globally-wrapper__item {
    gap: 10px;
    .globally-item__title {
      font-size: 12px;
    }
  }
}
.globally-btn {
  padding: 10px 25px;
  font-size: 11px;
}
@media screen and (max-width: 576px) {
  .globally-wrapper__item {
    display: flex;
    flex-direction: column;
    gap: 30px;
  }
  .globally-card-wrapper {
    flex-direction: column;
  }
}
</style>
