<template>
  <div class="navbar">
    <div class="container">
      <div class="navbar-wrapper">
        <div class="navbar-wrapper__image">
          <img src="@/assets/img/Group1.png" alt="" />
        </div>
        <div class="navbar-wrapper__item">
          <div class="navbar-wrapper__title">
            <p>Home</p>
            <p>Events</p>
            <p>About</p>
            <p>Blog</p>
            <p>Contact</p>
          </div>
          <div class="navbar-wrapper__btn">
            <button class="navbar-btn">
              <div class="navbar-img">
                <img src="@/assets/img/phone.svg" alt="" />
              </div>
              +998 91 207 6760
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style scoped lang="scss">
.navbar {
  padding: 50px 0px;
  background: #f0c53e;
}
.navbar-wrapper {
  display: flex;
  justify-content: space-between;
}
.navbar-wrapper__image img {
  width: 100%;
}
.navbar-wrapper__item {
  display: flex;
  gap: 50px;
  align-items: center;
}
.navbar-wrapper__title {
  display: flex;
  font-size: 20px;
  gap: 30px;
}
.navbar-img img {
  width: 70%;
  padding: 10px;
}
.navbar-btn {
  display: flex;
  border-radius: 30px;
  padding: 0px 15px 0px 5px;
  align-items: center;
  font-size: 12px;
  background: #b25a59;
  color: white;
  border: none;
  cursor: pointer;
}
.navbar-btn:active {
  font-size: 20px;
  color: white;
  background: #343232;
}
@media screen and (max-width: 992px) {
  .navbar-wrapper__title {
    font-size: 15px;
    gap: 10px;
  }
  .navbar-wrapper__item {
    display: flex;
    flex-direction: column;
    gap: 20px;
  }
  .navbar-btn {
    padding: 0px 10px;
    font-size: 12px;
  }
  .navbar-img img {
    width: 70%;
    padding: 5px;
  }
  .navbar-wrapper__image img {
    width: 80%;
  }
  .navbar-wrapper {
    display: flex;
    justify-content: space-around;
    align-items: center;
  }
}
@media screen and (max-width: 576px) {
  .navbar-wrapper {
    display: flex;
    flex-direction: column;
    text-align: center;
    gap: 20px;
  }
  .navbar-wrapper__title {
    font-size: 18px;
    gap: 10px;
  }
}
</style>
