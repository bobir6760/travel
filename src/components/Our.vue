<template>
  <div class="our">
    <div class="container">
      <div class="our-wrapper">
        <div class="our-info">
          <div class="our-info__title"><span>Our</span> Team</div>
          <div class="our-info__subtitle">
            Lorem Ipsum is simply dummy text of the printing and typesetting
            industry.
          </div>
        </div>
        <div class="our-wrapper__item">
          <div class="our-wrapper__image">
            <img src="@/assets/img/humans.png" alt="" />
          </div>
          <div class="our-item">
            <div class="our-item__title">
              Our <span>team is the secret</span> to our <br />success
            </div>
            <div class="our-wrapper__block">
              <div class="our-item__block">
                <div class="our-block__image">
                  <img src="@/assets/img/Group 72.svg" alt="" />
                </div>
                <div class="our-block__title">
                  Lorem Ipsum is simply dummy text of <br />the printing and
                  typesetting industry.<br />
                  Lorem Ipsum has been the industry's <br />standard dummy text
                  ever since the 1500s,
                </div>
              </div>
              <div class="our-item__block">
                <div class="our-block__image">
                  <img src="@/assets/img/Group 73.svg" alt="" />
                </div>
                <div class="our-block__title">
                  Lorem Ipsum is simply dummy text of <br />the printing and
                  typesetting industry.<br />
                  Lorem Ipsum has been the industry's <br />standard dummy text
                  ever since the 1500s,
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Our",
};
</script>

<style lang="scss" scoped>
.our {
  padding: 50px 0px;
}
$fz: 50px;
$color-1: #7f2736;
.our-wrapper {
  display: flex;
  flex-direction: column;
  gap: $fz;
}
.our-wrapper__item {
  display: flex;
  align-items: center;
  .our-item__title {
    cursor: pointer;
    span {
      color: $color-1;
    }
    font-weight: bold;
    font-size: 26px;
  }
}
.our-wrapper__image img {
  width: 90%;
  cursor: pointer;
}
.our-info {
  display: flex;
  flex-direction: column;
  gap: 20px;
  text-align: center;
  .our-info__title {
    font-size: 22px;
    font-weight: bold;
    span {
      color: $color-1;
    }
  }
  .our-info__subtitle {
    font-size: 18px;
  }
}
.our-item {
  display: flex;
  flex-direction: column;
  gap: $fz;
  .our-item__block {
    display: flex;
    gap: 20px;
    .our-block__title {
      font-size: 18px;
    }
  }
  .our-block__image img {
    width: 100%;
    cursor: pointer;
  }
  .our-block__image {
    padding: 5px;
    background: white;
    border-radius: 30px;
    border: 1px solid #fff;
    box-sizing: border-box;
  }
}
@media screen and (max-width: 1200px) {
  .our-info {
    gap: 20px;
  }
  .our-wrapper__item .our-item__title {
    font-size: 20px;
  }
  .our-item .our-item__block .our-block__title {
    font-size: 15px;
  }
}
@media screen and (max-width: 992px) {
  .our-wrapper__item .our-item__title {
    font-size: 17px;
  }
  .our-item .our-item__block .our-block__title {
    font-size: 12px;
  }
  .our-item .our-item__block {
    gap: 6px;
  }
  .our-wrapper__item {
    display: flex;
    flex-direction: column;
    text-align: center;
    gap: $fz;
  }
  .our-wrapper__block {
    display: flex;
    gap: $fz;
    text-align: start;
  }
}
@media screen and (max-width: 768px) {
  .our-info .our-info__subtitle {
    font-size: 15px;
  }
  .our-wrapper__block {
    display: flex;
    gap: 20px;
    text-align: start;
  }
  .our-info .our-info__title {
    font-size: 20px;
  }
}
@media screen and (max-width: 576px) {
  .our-wrapper__block {
    display: flex;
    flex-direction: column;
    gap: 20px;
    text-align: start;
  }
  .our-item .our-item__block .our-block__title {
    font-size: 14px;
  }
  .our-item {
    gap: 20px;
  }
}
</style>
