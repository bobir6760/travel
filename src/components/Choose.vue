<template>
  <div class="choose">
    <div class="container">
      <div class="choose-wrapper">
        <div class="choose-info">
          <div class="choose-info__title"><span>Why</span> Choose Us</div>
          <div class="choose-info__subtitle">
            Lorem Ipsum is simply dummy text of the printing and typesetting<br />
            industry. Lorem Ipsum has been the industry's standard dummy text<br />
            ever since the 1500s.
          </div>
        </div>
        <div class="choose-item">
          <div class="choose-wrapper__item">
            <div class="choose-block__image">
              <div class="choose-wrapper__image">
                <img src="@/assets/img/Vector1.svg" alt="" />
              </div>
            </div>
            <div class="choose-item__title">Handpicked Hotels</div>
            <div class="choose-item__subtitle">
              Lorem ipsum dolor sit amet, <br />consect adipiscing elit. Aenean
              <br />
              commodo ligula eget dolor. <br />Aenean massa
            </div>
          </div>
          <div class="choose-wrapper__item">
            <div class="choose-block__image">
              <div class="choose-wrapper__image">
                <img src="@/assets/img/Vector2.svg" alt="" />
              </div>
            </div>
            <div class="choose-item__title">World Class Service</div>
            <div class="choose-item__subtitle">
              Lorem ipsum dolor sit amet, <br />consect adipiscing elit. Aenean
              <br />
              commodo ligula eget dolor. <br />Aenean massa
            </div>
          </div>
          <div class="choose-wrapper__item">
              <div class="choose-wrapper__image">
                <img src="@/assets/img/Vector3.svg" alt="" />
              </div>
            <div class="choose-item__title">Best Price Guarantee</div>
            <div class="choose-item__subtitle">
              Lorem ipsum dolor sit amet, <br />consect adipiscing elit. Aenean
              <br />
              commodo ligula eget dolor. <br />Aenean massa
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Choose",
};
</script>

<style lang="scss" scoped>
.choose {
  padding: 50px 0px;
}
.choose-wrapper {
  display: flex;
  flex-direction: column;
  text-align: center;
  gap: 20px;
}
.choose-info {
  display: flex;
  flex-direction: column;
  gap: 20px;
  .choose-info__title {
    span {
      color: #7f2736;
    }
    font-weight: bold;
    font-size: 30px;
  }
}
.choose-item {
  display: flex;
  justify-content: center;
  gap: 50px;
  .choose-wrapper__item {
    display: flex;
    flex-direction: column;
    gap: 30px;
    padding: 30px;
    border-radius: 20px;
    background: #ffffff;
    box-shadow: 0px 10px 60px rgba(38, 45, 118, 0.08);
  }
  .choose-item__title {
    color: #7f2736;
    font-size: 22px;
    font-weight: bold;
  }
}
.choose-wrapper__image {
  display: flex;
  justify-content: center;
  padding: 5px;
  background: #ee5060;
  border-radius: 30px;
}
.choose-wrapper__image img {
  object-fit: contain;
  width: 40px;
  height: 40px;
}
@media screen and (max-width: 1200px) {
  .choose-item__subtitle {
    font-size: 16px;
  }
  .choose-item {
    gap: 20px;
  }
}
@media screen and (max-width: 992px) {
  .choose-item__subtitle {
    font-size: 12px;
  }
  .choose-item .choose-wrapper__item {
    gap: 15px;
  }
  .choose-item .choose-item__title {
    font-size: 18px;
  }
  .choose-info__subtitle {
    font-size: 15px;
  }
  .choose-info .choose-info__title {
    font-size: 25px;
  }
  .choose-wrapper__image img {
    object-fit: contain;
    width: 30px;
    height: 30px;
  }
}
@media screen and (max-width: 768px) {
  .choose-item__subtitle {
    font-size: 8px;
  }
  .choose-item .choose-item__title {
    font-size: 14px;
  }
  .choose-wrapper__image img {
    object-fit: contain;
    width: 20px;
    height: 20px;
  }
  .choose-info .choose-info__title {
    font-size: 20px;
  }
}
@media screen and (max-width: 576px) {
  .choose-item {
    display: flex;
    flex-direction: column;
  }
   .choose-item__subtitle {
    font-size: 12px;
  }
    .choose-item .choose-item__title {
    font-size: 18px;
  }
    .choose-info .choose-info__title {
    font-size: 25px;
  }
}
</style>
