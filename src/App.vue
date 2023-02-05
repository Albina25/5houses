<template>
  <div id="app">
    <header class="header-block container">
      <div class="logo">
        <a href="#"><img src="./assets/logo1.png" alt="logo" /></a>
      </div>
      <div class="main-menu">
        <ul class="main-menu__list">
          <li class="active main-menu__item">
            <a class="text-uppercase main-menu__item_link" href="#">меню</a>
          </li>
          <!--<li><a href="#">lifestyle</a></li>
          <li><a href="#">Food</a></li>
          <li><a href="#">Nature</a></li>
          <li><a href="#">photography</a></li>-->
        </ul>
      </div>
      <div class="">Войти</div>
    </header>
    <main class="main-block">
      <section class="main-block__head container">
        <div class="main-block__head-content container">
          <p class="main-block__head-title">Отдыхай с удовольствием</p>
        </div>
      </section>
      <section class="main-block__content container">
        <div class="main-block__part">
          <div class="main-block__info">
            <h3>Информация</h3>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam.eiusmod tempor incididunt ut labore et dolore
              magna aliqua. Ut enim ad minim veniam.
            </p>
          </div>
          <div class="main-block__info">
            <h3>Цены</h3>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam.eiusmod tempor incididunt ut labore et dolore
              magna aliqua. Ut enim ad minim veniam.
            </p>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam.eiusmod tempor incididunt ut labore et dolore
              magna aliqua. Ut enim ad minim veniam.
            </p>
          </div>
          <div id="test" class="main-block__info">
            <h3>Бронь</h3>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam.eiusmod tempor incididunt ut labore et dolore
              magna aliqua. Ut enim ad minim veniam.
            </p>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam.eiusmod tempor incididunt ut labore et dolore
              magna aliqua. Ut enim ad minim veniam.
            </p>
          </div>
        </div>
        <div class="main-block__part main-block__images">
          <div class="row">
            <div class="column">
              <img style="width: 100%" src="./uploads/abc.jpg" />
              <img style="width: 100%" src="./uploads/p2.jpg" />
              <img style="width: 100%" src="./uploads/blog-grid.jpg" />
              <img style="width: 100%" src="./uploads/ins-2.jpg" />
              <img style="width: 100%" src="./uploads/ins-3.jpg" />
            </div>
            <div class="column">
              <img style="width: 100%" src="./uploads/blog-1.jpg" />
              <img style="width: 100%" src="./uploads/me-cover.jpg" />
              <img style="width: 100%" src="./uploads/footer-img.png" />
              <img style="width: 100%" src="./uploads/ins-4.jpg" />
              <img style="width: 100%" src="./uploads/blog-2.jpg" />
            </div>
          </div>
        </div>
      </section>
    </main>
    <footer class="footer-block container">
      <div class="footer-block__years">&copy; Пять домиков 2023</div>
      <!--<div class="col-md-6 text-center text-md-end"><?/*= Yii::powered() */?></div>-->
    </footer>
  </div>
</template>

<script>
export default {
  name: "App",
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  display: flex;
  flex-direction: column;
  //color: #2c3e50;
}
.header-block {
  background-color: var(--main-color, #063949);
  //box-shadow: 1px 1px 1px 1px #063949;
  height: var(--header-size, 65px);
  z-index: 10;
  width: 100%;
  position: fixed;
  top: 0;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.container {
  padding: 0 2rem;
  margin: 0 auto;
  max-width: 100%;
}
.logo {
  display: flex;
  height: 60px;
  border-radius: 2px;
  align-items: center;
}
.col-2 {
  flex: 0 0 16%;
  max-width: 16%;
}
.main-menu {
  text-align: center;

  &__item {
    display: inline-block;
    margin-right: -4px;
  }

  &__item_link {
    color: #d6d3d9;
    text-decoration: none;
    text-transform: uppercase;
    padding: 0 15px;
    font-weight: 700;
    font-size: 1rem;
    line-height: 65px;
    display: block;
    transition: background-color 0.22s linear, color 0.22s linear;
    border-radius: 2px;
  }
}
.main-block {
  &__head {
    position: relative;
    z-index: 0;
    background-image: url("./assets/images/main-photo1.jpg");
    min-height: 700px;

    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;

    color: #ffffff;

    &:before {
      content: "";
      position: absolute;
      z-index: -1;
      display: block;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(var(--main-color-rgb), 0.1);
      background-image: linear-gradient(to bottom, transparent, rgb(0 0 0/1));
    }
    &-content {
      position: absolute;
      //width: 100%;
      display: inline-block;
      max-width: 910px;
      bottom: 15%;
      left: 0;
      //padding-left: 40px;
    }
    &-title {
      font-size: 32px;
      line-height: 1.2;
      margin-top: 20px;
      margin-bottom: 19px;
      display: block;
      font-weight: 700;
    }
  }
  &__content {
    margin-top: 2rem;
    display: flex;
    flex-direction: row;
    width: 100%;
  }
  &__part {
    width: 50%;
  }
  &__info {
    background-color: #fff;
    padding: 4px;
    border: 1px solid #ececec;
    position: relative;
    box-shadow: 0 4px 40px rgb(10 0 0 / 8%);
    margin-bottom: 0.5rem;
    text-align: left;
  }
  &__images {
    background-color: #fff;
    padding: 4px;
    border: 1px solid #ececec;
    position: relative;
    box-shadow: 0 4px 40px rgb(10 0 0 / 8%);
  }
  .row {
    display: flex;
    flex-wrap: wrap;
    padding: 0 4px;
  }

  .column {
    flex: 50%;
    padding: 0 4px;
  }

  .column img {
    margin-top: 8px;
    vertical-align: middle;
  }
}
.footer-block {
  width: 100%;
  display: flex;
  height: var(--header-size);
  align-items: center;
}
@media (max-width: 768px) {
  .container {
    padding: 0 1rem;
  }
  .main-block {
    &__content {
      flex-direction: column;
    }
    &__part {
      width: 100%;
    }
  }
}
</style>
