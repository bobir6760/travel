<template>
  <div class="write">
    <div class="container">
      <div class="write-wrapper">
        <div class="write-wrapper__item">
          <div class="write-info">
            <div class="write-info__title">TESTIMONIAL</div>
            <div class="write-info__subtitle">What Customers Say?</div>
            <div class="write-info__text">
              <p>
                Lorem Ipsum is simply dummy text of the <br />printing and
                typesetting industry.
              </p>
              <p>
                Lorem Ipsum is simply dummy text of the <br />printing and
                typesetting industry.
              </p>
              <p>Lorem Ipsum is simply dummy text of the</p>
            </div>
            <div class="write-btn">
              <button class="write-info__btn">Write your thought</button>
            </div>
          </div>
          <div class="write-item">
            <div class="write-item__image">
              <img src="@/assets/img/Mask.png" alt="" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Write",
};
</script>

<style lang="scss" scoped>
.write {
  padding: 50px 0px;
}
.write-wrapper {
  display: flex;
  flex-direction: column;
  gap: 50px;
  .write-wrapper__item {
    display: flex;
    justify-content: space-between;
  }
}
.write-info {
  display: flex;
  flex-direction: column;
  gap: 40px;
  .write-info__title {
    font-size: 12px;
    font-weight: bold;
    cursor: pointer;
  }
  .write-info__subtitle {
    color: #7f2736;
    font-size: 40px;
    font-weight: bold;
    cursor: pointer;
  }
  .write-info__text {
    display: flex;
    flex-direction: column;
    gap: 15px;
    font-size: 18px;
    cursor: pointer;
  }
  .write-info__btn {
    padding: 10px 60px 10px 20px;
    border-radius: 30px;
    color: #ee5060;
    background: white;
    border-color: #ee5060;
    cursor: pointer;
    font-size: 14px;
  }
   .write-info__btn:hover {
    background: #7f2736;
    color: white;
    transition: 0.9s;
  }
}
.write-item {
  display: flex;
  .write-item__image img {
    display: flex;
    width: 80%;
  }
  .write-item__image {
    display: flex;
    border-radius: 20px;
    overflow: hidden;
    justify-content: center;
    cursor: pointer;
  }
}
.write-block {
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  gap: 50px;
  padding: 20px;
  background: #ffffff;
  box-shadow: 2px 4px 60px rgba(41, 44, 124, 0.1);
  border-radius: 20px;
  width: 50%;
  .write-block__title {
    font-size: 20px;
    cursor: pointer;
  }
}
.write-block__image {
  display: flex;
  flex-direction: column;
  gap: 10px;
  cursor: pointer;
  .write-image img {
    object-fit: contain;
    width: 30px;
    height: 30px;
    cursor: pointer;
  }
}
.write-wrapper__block {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.write-block__item {
  display: flex;
  gap: 5px;
}
.write-block__text {
  font-size: 18px;
  color: #80819a;
}
.write-block__subtitle {
  font-size: 20px;
  font-weight: bold;
}
@media screen and (max-width: 1200px) {
  .write-block .write-block__title {
    font-size: 16px;
  }
  .write-block {
    gap: 20px;
  }
  .write-item .write-item__image img {
    width: 70%;
  }
}
@media screen and (max-width: 992px) {
  .write-item .write-item__image {
    display: flex;
    justify-content: center;
  }
  .write-item .write-item__image img {
    width: 80%;
  }
  .write-info .write-info__subtitle {
    font-size: 25px;
  }
  .write-info__text p {
    font-size: 17px;
  }
  .write-info .write-info__btn {
    font-size: 14px;
  }
  .write-block .write-block__title {
    font-size: 12px;
  }
  .write-block__image .write-image img {
    object-fit: contain;
    width: 20px;
    height: 20px;
  }
  .write-block__image {
    gap: 5px;
  }
  .write-block__subtitle {
    font-size: 20px;
  }
}
@media screen and (max-width: 768px) {
  .write-info__text p {
    font-size: 12px;
  }
  .write-info .write-info__btn {
    font-size: 14px;
    padding: 10px 17px 10px 10px;
  }
  .write-info .write-info__subtitle {
    font-size: 20px;
  }
  .write-block__subtitle {
    font-size: 16px;
  }
  .write-block__image {
    gap: 0px;
  }
}
@media screen and (max-width: 576px) {
  .write-wrapper__item {
    display: flex;
    flex-direction: column;
    text-align: center;
    gap: 30px;
  }
  .write-block {
    display: flex;
    flex-direction: column;
    width: 100%;
  }
  .write-info .write-info__subtitle {
    font-size: 25px;
  }
  .write-info__text p {
    font-size: 15px;
  }
}
</style>
