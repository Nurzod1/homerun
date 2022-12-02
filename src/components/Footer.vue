<template>
  <div class="footer">
    <div class="container">
      <div class="footer-wrapper">
        <div class="footer-intro">
          <div class="footer-intro__logo">
            <img src="../assets/img/logo5.png" alt="" />
          </div>
          <Button title="Start free trial" />
        </div>
        <div class="footer-menu__wrapper">
          <div class="footer-menu">
            <div class="footer-menu1">
              <div class="footer-menu__title">Product</div>
              <div class="footer-menu__link1">Hire</div>
              <div class="footer-menu__link2">Create</div>
              <div class="footer-menu__link">Templates</div>
              <div class="footer-menu__link">All features</div>
            </div>
            <div class="footer-menu1">
              <div class="footer-menu__link">Pricing</div>
              <div class="footer-menu__link">New in Homerun✨</div>
            </div>
          </div>
          <div class="footer-menu">
            <div class="footer-menu1">
              <div class="footer-menu__title">Learn</div>
              <div class="footer-menu__link">Blog</div>
              <div class="footer-menu__link">Help Center</div>
            </div>
            <div class="footer-menu1">
              <div class="footer-menu__title">Guides</div>
              <div class="footer-menu__link">Remote Hiring</div>
              <div class="footer-menu__link">Employer Branding</div>
              <div class="footer-menu__link">Job Interviewing</div>
              <div class="footer-menu__link">Diversity & Inclusion</div>
              <div class="footer-menu__link">Attracting Talent</div>
              <div class="footer-menu__link">GDPR Hiring</div>
            </div>
          </div>
          <div class="footer-menu">
            <div class="footer-menu1">
              <div class="footer-menu__title">About Homerun</div>
              <div class="footer-menu__link">About us</div>
              <div class="footer-menu__link">We're hiring</div>
              <div class="footer-menu__link">Contact us</div>
            </div>
            <div class="footer-menu1">
              <div class="footer-menu__title">Legal</div>
              <div class="footer-menu__link">Terms</div>
              <div class="footer-menu__link">Privacy</div>
            </div>
          </div>
          <div class="sign">
            <div class="sign-about">
              <div class="sign-about__title">Art of Work newsletter</div>
              <div class="sign-about__text">
                Receive must-read articles and trends on company culture, hiring
                and work/life balance.
              </div>
            </div>
            <div class="sign-input">
              <div class="sign-input__text">Sign up to our newsletter</div>
              <div class="sign-input__signup">
                <input type="text" />
                <button>send</button>
              </div>
            </div>
            <div class="sign-contacts">
              <div class="sign-contacts__link">
                <img src="../assets/img/insta.png" alt="" />
              </div>
              <div class="sign-contacts__link">
                <img src="../assets/img/linkedin.png" alt="" />
              </div>
              <div class="sign-contacts__link">
                <img src="../assets/img/twitter.png" alt="" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Button from "./Button.vue";
export default {
  components: { Button },
  name: "Footer",
};
</script>

<style lang="scss" scoped>
.footer {
  margin: 100px 0;
  color: #fff;
  &-wrapper {
    display: flex;
    flex-direction: column;
    gap: 40px;
    background-color: #000;
    border-radius: 20px;
    padding: 40px;
  }
  &-intro {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
  &-menu {
    display: flex;
    flex-direction: column;
    gap: 40px;
    &__wrapper {
      display: flex;
      justify-content: space-between;
      @include breakpoint(md) {
        display: grid;
        grid-template-columns: 1fr 1fr;
        gap: 140px;
        justify-content: space-between;
      }
      @include breakpoint(md) {
        gap: 50px;
      }
      @include breakpoint(md) {
        gap: 10px;
      }
    }
    &__title {
      font-size: 18px;
      line-height: 24px;
      font-weight: 700;
      @include breakpoint(md) {
        font-size: 16px;
        line-height: 22px;
      }
    }
    &__link {
      font-size: 18px;
      line-height: 25px;
      color: #778291;
      cursor: pointer;
      transition: 0.3s;
      &:hover {
        color: #fff;
      }
      @include breakpoint(md) {
        font-size: 16px;
        line-height: 22px;
      }
    }
    &__link1 {
      font-size: 18px;
      line-height: 25px;
      color: #0c9f64;
      font-weight: 700;
      cursor: pointer;
      transition: 0.3s;
      &:hover {
        color: #fff;
      }
      @include breakpoint(md) {
        font-size: 16px;
        line-height: 22px;
      }
    }
    &__link2 {
      font-size: 18px;
      line-height: 25px;
      color: #fec104;
      font-weight: 700;
      cursor: pointer;
      transition: 0.3s;
      &:hover {
        color: #fff;
      }
      @include breakpoint(md) {
        font-size: 16px;
        line-height: 22px;
      }
    }
  }
  &-menu1 {
    display: flex;
    flex-direction: column;
    gap: 20px;
    @include breakpoint(xs) {
      gap: 10px;
    }
  }
  .sign {
    display: flex;
    flex-direction: column;
    gap: 30px;
    &-about {
      display: flex;
      flex-direction: column;
      gap: 20px;
      @include breakpoint(xs) {
        gap: 10px;
      }
      &__title {
        font-size: 18px;
        line-height: 27px;
        font-weight: 700;
        @include breakpoint(md) {
          font-size: 16px;
          line-height: 24px;
        }
      }
      &__text {
        font-size: 20px;
        line-height: 28px;
        max-width: 307px;
        @include breakpoint(md) {
          font-size: 14px;
          line-height: 22px;
        }
      }
    }
    &-input {
      display: flex;
      flex-direction: column;
      gap: 13px;
      @include breakpoint(xs) {
        gap: 10px;
      }
      &__text {
        font-size: 20px;
        line-height: 28px;
        @include breakpoint(xs) {
          font-size: 16px;
          line-height: 20px;
        }
      }
      &__signup {
        display: flex;
        input {
          border-radius: 8px 0px 0px 8px;
          background-color: rgba(119, 130, 145, 0.3);
          border: none;
          width: 256px;
          height: 40px;
          color: #fff;
          padding: 5px;
          font-size: 20px;
          line-height: 26px;
          outline: none;
          @include breakpoint(md) {
            width: 156px;
          }
          @media screen and (max-width: 539px) {
            width: 86px;
            height: 20px;
          }
          &::placeholder {
            color: #b2b2b2;
          }
        }
        button {
          background-color: #595d68;
          width: 78px;
          height: 40px;
          border-radius: 0px 8px 8px 0px;
          border: none;
          color: #fff;
          font-size: 20px;
          line-height: 25px;
          @include breakpoint(md) {
            width: 48px;
          }
          @media screen and (max-width: 539px) {
            width: 38px;
            height: 20px;
          }
        }
      }
    }
    &-contacts {
      display: flex;
      gap: 10px;
      @media screen and (max-width: 340px) {
        gap: 5px;
      }
    }
  }
}
</style>