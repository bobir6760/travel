<template>
  <div class="finish">
    <div class="container">
      <div class="finish-wrapper">
        <div class="finish-info">
          <div class="finish-wrapper-card">
            <div class="finish-card__image">
              <img src="@/assets/img/Group7.png" alt="" />
            </div>
            <div class="finish-info__title">
              Domestic <br />International <br />Tours
            </div>
          </div>
          <div class="finish-body-card">
            <div class="finish-body__title">
              Subscribe to get our Newsletter
            </div>
            <div class="finish-body__block">
              <div class="finish-input">
                <input placeholder="Your Name" type="text" />
              </div>
              <div class="finish-body__item">
                <button class="Finish-btn">Subscribe</button>
              </div>
            </div>
          </div>
          <div class="finish-card__text">
            <div class="finish-text__title">
              <p>Careers</p>
              <p>Privacy Policy</p>
              <p>Terms & Conditions</p>
            </div>
            <div class="finish-card__subtitle">© 2021 Tourism Department.</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Finish",
};
</script>

<style scoped lang="scss">
.finish {
  padding: 50px 0px;
  background: #7f2736;
}
.finish-wrapper {
  display: flex;
  justify-content: center;
}
.finish-info {
  display: flex;
  flex-direction: column;
  gap: 50px;
  .finish-wrapper-card {
    display: flex;
    align-items: center;
    gap: 2 0px;
    .finish-info__title {
      color: white;
      font-size: 20px;
      font-weight: bold;
    }
    .finish-card__image img {
      width: 80%;
    }
  }
}
.finish-body-card {
  display: flex;
  flex-direction: column;
  text-align: center;
  gap: 10px;
  .finish-body__title {
    font-size: 22px;
    font-weight: bold;
    color: #f0c53e;
  }
  .finish-body__block {
    display: flex;
    gap: 15px;
    .finish-input input {
      background: #7f2736;
      padding: 10px 80px 10px 15px;
      font-size: 16px;
      border-radius: 20px;
      border-color: #f0c53e;
      color: white;
    }
    .Finish-btn {
      cursor: pointer;
      padding: 12px 22px;
      border-radius: 20px;
      border: none;
      font-size: 16px;
      color: white;
      background: linear-gradient(105.5deg, #ee5060 19.57%, #b25a59 78.85%);
    }
    .Finish-btn:active {
      color: #f0c53e;
    }
  }
}
.finish-card__text {
  display: flex;
  flex-direction: column;
  text-align: center;
  gap: 20px;
  .finish-text__title {
    display: flex;
    font-size: 20px;
    gap: 30px;
    color: #f0c53e;
  }
  .finish-card__subtitle {
    font-size: 20px;
    color: #f0c53e;
  }
}
@media screen and (max-width: 576px) {
  .finish-body__block {
    display: flex;
    flex-direction: column;
  }
  .finish-card__text {
    gap: 7px;
  }
  .finish-card__text .finish-text__title {
    display: flex;
    font-size: 15px;
    gap: 18px;
  }
  .finish-info {
    gap: 40px;
  }
}
</style>
