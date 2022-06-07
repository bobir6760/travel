<template>
  <div class="news">
    <div class="container">
      <div class="news-wrapper">
        <div class="news-info">
          <div class="news-info__title">Lastest News and Resources</div>
          <div class="news-info__subtitle">
            Lorem Ipsum is simply dummy text of the printing and typesetting
            industry.
          </div>
        </div>
        <div class="news-wrapper__item">
          <div class="news-item__block">
            <div class="news-block__image">
              <img src="@/assets/img/CITY.png" alt="" />
            </div>
            <div class="news-item__btn">
              <button class="news-btn">NEWS</button>
            </div>
            <div class="news-block__title">Where does it come from?</div>
            <div class="news-block__subtitle">
              Contrary to popular belief, Lorem Ipsum is not simply <br />random
              text. It has roots in a piece of classical Latin <br />literature
              from 45 BC, making it over 2000 years old.
            </div>
            <div class="news-block__text">Read more</div>
          </div>

          <div class="news-item">
            <div class="news-text__block">
              <div class="news-item__image">
                <img src="@/assets/img/gara.jpg" alt="" />
              </div>
              <div class="news-item__body">
                <div class="news-item__title">Where does it come from?</div>
                <div class="news-item__subtitle">
                  Contrary to popular belief, Lorem Ipsum is <br />not simply
                  random text. It has roots in a <br />piece of classical Latin
                  literature from 45 <br />BC, making it over 2000 years old.
                </div>
              </div>
            </div>
            <div class="news-text__block">
              <div class="news-item__image">
                <img src="@/assets/img/gara.jpg" alt="" />
              </div>
              <div class="news-item__body">
                <div class="news-item__title">Where does it come from?</div>
                <div class="news-item__subtitle">
                  Contrary to popular belief, Lorem Ipsum is <br />not simply
                  random text. It has roots in a <br />piece of classical Latin
                  literature from 45 <br />BC, making it over 2000 years old.
                </div>
              </div>
            </div>
            <div class="news-text__block">
              <div class="news-item__image">
                <img src="@/assets/img/gara.jpg" alt="" />
              </div>
              <div class="news-item__body">
                <div class="news-item__title">Where does it come from?</div>
                <div class="news-item__subtitle">
                  Contrary to popular belief, Lorem Ipsum is <br />not simply
                  random text. It has roots in a <br />piece of classical Latin
                  literature from 45 <br />BC, making it over 2000 years old.
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
  name: "News",
};
</script>

<style lang="scss" scoped>
.news {
  padding: 50px 0px;
}
.news-wrapper {
  display: flex;
  flex-direction: column;
  gap: 50px;
}
.news-info {
  display: flex;
  flex-direction: column;
  text-align: center;
  gap: 30px;
  .news-info__title {
    font-size: 25px;
    color: #7f2736;
    font-weight: bold;
  }
  .news-info__subtitle {
    font-size: 20px;
  }
}
.news-item__block {
  display: flex;
  flex-direction: column;
  gap: 30px;
  .news-block__title {
    color: #7f2736;
    font-weight: bold;
    font-size: 22px;
  }
  .news-block__subtitle {
    font-size: 18px;
  }
  .news-block__text {
    font-size: 20px;
    letter-spacing: 0.02em;
    text-decoration-line: underline;
    color: #ee5060;
  }
}
.news-block__image {
  display: flex;
  overflow: hidden;
  border-radius: 20px;
}
.news-block__image img {
  width: 100%;
}
.news-btn {
  background: #f0c53e;
  padding: 10px 40px;
  border-radius: 20px;
  border: none;
  font-size: 18px;
  font-weight: bold;
  cursor: pointer;
}
.news-btn:active {
  color: white;
  background: #343232;
}
.news-item {
  display: flex;
  flex-direction: column;
  gap: 30px;
  .news-text__block {
    display: flex;
    gap: 20px;
    align-items: center;
  }
}
.news-item__image {
  display: flex;
  overflow: hidden;
  border-radius: 20px;
}
.news-item__image img {
  width: 100%;
}
.news-wrapper__item {
  display: flex;
  justify-content: space-between;
  gap: 50px;
}
.news-item__body {
  display: flex;
  flex-direction: column;
  gap: 20px;
  .news-item__title {
    color: #7f2736;
    font-weight: bold;
  }
  .news-item__subtitle {
    font-size: 15px;
  }
}
@media screen and (max-width: 1200px) {
  .news-item__block .news-block__subtitle {
    font-size: 15px;
  }
  .news-item__body .news-item__subtitle {
    font-size: 14px;
  }
}
@media screen and (max-width: 992px) {
  .news-item__block .news-block__subtitle {
    font-size: 11px;
  }
  .news-item__body .news-item__subtitle {
    font-size: 11px;
  }
  .news-item__body .news-item__title {
    color: #7f2736;
    font-weight: bold;
    font-size: 17px;
  }
  .news-item__body {
    gap: 10px;
  }
  .news-btn[data-v-293a9583] {
    padding: 8px 30px;
    font-size: 15px;
  }
}
@media screen and (max-width: 768px) {
  .news-item__body .news-item__title {
    font-size: 15px;
  }
  .news-item__block .news-block__subtitle {
    font-size: 9px;
  }
  .news-item__body .news-item__subtitle {
    font-size: 5px;
  }
  .news-item__block {
    gap: 10px;
  }
  .news-wrapper {
    gap: 30px;
  }
  .news-info .news-info__subtitle {
    font-size: 15px;
  }
  .news-info .news-info__title {
    font-size: 23px;
  }
}
@media screen and (max-width: 576px) {
  .news-wrapper__item {
    display: flex;
    flex-direction: column;
  }
  .news-item__block {
    gap: 20px;
    text-align: center;
  }
  .news-item .news-text__block {
    gap: 10px;
    display: flex;
    flex-direction: column;
  }
  .news-item__body .news-item__title {
    font-size: 20px;
  }
  .news-item__body .news-item__subtitle {
    font-size: 14px;
    text-align: center;
  }
  .news-info {
    gap: 20px;
  }
}
</style>
