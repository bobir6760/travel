<template>
  <div class="best">
    <div class="container">
      <div class="best-wrapper">
        <div class="best-info">
          <div class="best-wrapper__title">
            <span>Life is a journey</span>, not a <br />destination
          </div>
          <div class="best-wrapper__subtitle">
            Let’s start your journey with us, your dream will <br />come true...
          </div>
          <div class="best-wrapper__item">
            <div class="best-wrapper__btn">
              <button class="best-btn">Explore Destinations</button>
            </div>
            <div class="best-item">
              <div class="best-item__image">
                <img src="@/assets/img/Polygon.svg" alt="" />
              </div>
              <div class="best-item__title">Watch how it works</div>
            </div>
          </div>
        </div>
        <div class="best-block">
          <div class="best-wrapper__body">
            <div class="best-wrapper__image odd">
              <img src="@/assets/img/calendar.svg" alt="" />
            </div>
            <div class="best-wrapper__text">
              <div class="best-body__title">250k</div>
              <div class="best-body__subtitle">Plan Your Trip</div>
            </div>
          </div>
          <div class="best-wrapper__body">
            <div class="best-wrapper__image">
              <img src="@/assets/img/Group2.svg" alt="" />
            </div>
            <div class="best-wrapper__text">
              <div class="best-wrapper__block">
                <div class="best-body__title">Upcoming Trips</div>
                <div class="best-body__subtitle">Today at 12.00 PM</div>
              </div>
              <div class="best-body__btn">
                <button class="best-body__btn">Join Now</button>
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
  name: "Best",
};
</script>

<style scoped lang="scss">
.best {
  padding: 50px 0px;
  background: #f0c53e;
}
$fz: 10px;
.best-wrapper {
  display: flex;
  justify-content: space-around;
  gap: 40px;
}
.best-info {
  display: flex;
  flex-direction: column;
  gap: 40px;
}
.best-wrapper__title {
  font-size: 40px;
  cursor: pointer;
  span {
    color: #7f2736;
    font-weight: bold;
  }
}
.best-wrapper__title:hover {
  text-decoration: underline;
}
.best-wrapper__subtitle {
  font-size: 20px;
  cursor: pointer;
}

.best-wrapper__item {
  display: flex;
  gap: 20px;
  align-items: center;
}
.best-item {
  display: flex;
  gap: 20px;
  align-items: center;
}
.best-btn {
  color: white;
  background: #b25a59;
  border-radius: 30px;
  border: none;
  padding: 15px 25px;
  font-size: 12px;
  cursor: pointer;
  text-align: center;
}
.best-btn:active {
  color: #f0c53e;
}
.best-btn:hover {
  transition: 0.5s;
  box-shadow: inset 300px 0 0 0 black;
}
.best-item__image img {
  width: 100%;
  cursor: pointer;
}
.best-item__image {
  padding: 11px 9px 5px 17px;
  background: white;
  border-radius: 30px;
  border: 1px solid #fff;
  box-sizing: border-box;
}
.best-item__title {
  font-size: 20px;
  cursor: pointer;
  &:hover {
    color: #b25a59;
    text-decoration: underline black;
  }
}
.best-wrapper__image img {
  width: 100%;
  cursor: pointer;
}
.best-wrapper__image {
  padding: 10px;
  background: #ee5060;
  border-radius: 8px;
  cursor: pointer;
}
.best-wrapper__image {
  background: #f0c53e;
  border-radius: 8px;
  cursor: pointer;
}
.best-wrapper__body {
  display: flex;
  align-items: center;
  padding: 15px 60px 15px 10px;
  background: rgba(255, 255, 255, 0.8);
  border-radius: 15px;
  gap: 10px;
}
.best-block {
  display: flex;
  flex-direction: column;
  gap: 60px;
}
.best-body__title {
  font-size: 15px;
  font-weight: bold;
  cursor: pointer;
}
.best-body__btn {
  padding: 5px 20px;
  background: #b25a59;
  border-radius: 80px;
  border: none;
  font-size: $fz;
  color: #fff;
  cursor: pointer;
  text-align: center;
}
.best-body__btn:active {
  color: white;
}
.best-body__btn:hover {
  transition: 0.7s;
  background: #f0c53e;
  color: black;
}
.best-wrapper__block {
  margin-bottom: 20px;
  cursor: pointer;
}
@media screen and (max-width: 992px) {
  .best-wrapper__title {
    font-size: 35px;
  }
  .best-wrapper__body {
    padding: 15px 20px 15px 10px;
  }
}
@media screen and (max-width: 768px) {
  .best-wrapper__item {
    display: flex;
    flex-direction: column;
    gap: 20px;
  }
  .best-wrapper__title {
    font-size: 25px;
  }
  .best-wrapper__subtitle {
    font-size: 12px;
  }
}
@media screen and (max-width: 576px) {
  .best-wrapper {
    display: flex;
    flex-direction: column;
    gap: 40px;
  }
  .best-info {
    gap: 30px;
    text-align: center;
  }
  .best-wrapper__title {
    font-size: 30px;
  }
  .best-wrapper__subtitle {
    font-size: 14px;
  }
  .best-block {
    gap: 20px;
  }
}
</style>
