<template>
  <div class="citys">
    <div class="container">
      <div class="citys-wrapper">
        <div class="citys-info">
          <div class="citys-info__title">
            <span>Check Our Best</span> Promotional Tour
          </div>
          <div class="citys-info__subtitle">
            Lorem Ipsum is simply dummy text of the printing and typesetting
            <br />
            industry. Lorem Ipsum has been the industry's standard dummy text
            <br />
            ever since the 1500s, when an unknown printer took a galley of
            type<br />
            and scrambled it to make a type specimen book.
          </div>
        </div>

        <div class="citys-info__item">
          <div class="citys-item">
            <div class="citys-info__image">
              <img src="@/assets/img/CITY.png" alt="" />
            </div>
            <div class="citys-item__title">Beijing</div>
          </div>
          <div class="citys-item">
            <div class="citys-info__image">
              <img src="@/assets/img/CITY2.png" alt="" />
            </div>
            <div class="citys-item__title">Turkey</div>
          </div>
          <div class="citys-item">
            <div class="citys-info__image">
              <img src="@/assets/img/CITY3.png" alt="" />
            </div>
            <div class="citys-item__title">Pakistan</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Citys",
};
</script>

<style scoped lang="scss">
.citys {
  padding: 50px 0px;
  background: white;
}
.citys-wrapper {
  display: flex;
  flex-direction: column;
  gap: 50px;
}
.citys-info {
  display: flex;
  flex-direction: column;
  gap: 10px;
  text-align: center;
}
.citys-info__title {
  font-size: 25px;
  cursor: pointer;
  span {
    color: #7f2736;
  }
  font-weight: bold;
}
.citys-info__subtitle {
  font-size: 15px;
}
.citys-info__image img {
  width: 100%;
  cursor: pointer;
}
.citys-info__item {
  display: flex;
  text-align: center;
  gap: 30px;
}
.citys-info__image {
  display: flex;
  border-radius: 12px;
  overflow: hidden;
  cursor: pointer;
}
.citys-item {
  display: flex;
  flex-direction: column;
  gap: 20px;
}
.citys-item__title {
  color: #7f2736;
  font-weight: bold;
  cursor: pointer;
  &:hover {
    font-size: 25px;
    color: #343232;
    transition: 0.9s;
  }
}
@media screen and (max-width: 992px) {
  .citys-info__subtitle {
    font-size: 15px;
  }
}
@media screen and (max-width: 768px) {
  .citys-info__title {
    font-size: 22px;
  }
}
@media screen and (max-width: 576px) {
  .citys-info__item {
    display: flex;
    flex-direction: column;
    text-align: center;
    gap: 40px;
  }
  .citys-item {
    gap: 10px;
  }
  .citys-info__subtitle {
    font-size: 10px;
  }
}
</style>
