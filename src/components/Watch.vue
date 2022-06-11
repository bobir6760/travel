<template>
  <div class="watch">
    <div class="container">
      <div class="watch-wrapper">
        <div class="watch-info">
          <div class="watch-info__title">
            <span>Watch,</span> our lattest tour
          </div>
          <div class="watch-info__subtitle">
            Lorem Ipsum is simply dummy text of the printing and typesetting
            industry. Lorem Ipsum has been the industry's standard dummy text
            ever since the 1500s, when an unknown printer took a galley of type
            and scrambled it to make a type specimen book.
          </div>
          <div class="watch-info__text">Learn more</div>
        </div>
        <div class="watch-image">
          <div class="watch-wrapper__image">
            <img src="@/assets/img/Marmo.jpg" alt="" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Watch",
};
</script>

<style scoped lang="scss">
.watch {
  padding: 50px 0px;
}
$fz: 25px;
.watch-wrapper {
  display: flex;
  justify-content: space-between;
  gap: 50px;
}
.watch-info {
  display: flex;
  flex-direction: column;
  gap: 20px;
  .watch-info__title {
    font-size: 22px;
    cursor: pointer;
    span {
      color: #7f2736;
    }
  }
  .watch-info__subtitle {
    font-size: 15px;cursor: pointer;
  }
  .watch-info__text {
    color: #ee5060;
    text-decoration: underline;
    &:hover {
      color: #ee5060;
      font-size: $fz;
      transition: 0.9s;
      cursor: pointer;
    }
  }
}
.watch-wrapper__image img {
  width: 100%;
  cursor: pointer;
}
.watch-wrapper__image {
  display: flex;
  border-radius: 12px;
  overflow: hidden;
}
@media screen and (max-width: 768px) {
  .watch-wrapper {
    gap: 20px;
  }
}
@media screen and (max-width: 576px) {
  .watch-wrapper {
    display: flex;
    flex-direction: column;
    text-align: center;
  }
}
</style>
