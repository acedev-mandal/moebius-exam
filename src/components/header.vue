<template>
  <div>
    <div class="header">
      <div class="header-wrap">
        <nav class="header-nav-links">
          <div class="fl-left">
            <a class="home-logo" href="#">
              <img
                src="./../assets/images/moebius-logo-color.svg"
                alt="moebius-logo-color"
              />
            </a>
          </div>
          <div class="fl-right">
            <ul>
              <li><a href="#">home</a></li>
              <li><a href="#">service</a></li>
              <li><a href="#">about</a></li>
              <li><a href="#">jobs</a></li>
            </ul>
            <a class="contact-us" href="#">Contact Us</a>
          </div>
        </nav>
        <div class="header-welcome"><span>hello</span>Welcome to Mobius</div>
        <div class="header-big-text">reach your destination,</div>
        <div class="header-line-gradient"></div>
        <div class="header-msg">
          <p>
            We're email, e-commerce and fintech experts. We have a proven track
            record in delivering complex solutions to diverse industries.
          </p>
        </div>
        <div class="icons-bar">
          <ul>
            <li>
              <a href="#"
                ><img src="./../assets/images/group.svg" alt="group"
              /></a>
            </li>
            <li>
              <a href="#"
                ><img
                  src="./../assets/images/hydropay-icon.svg"
                  alt="hydropay-icon"
              /></a>
            </li>
            <li>
              <a href="#"
                ><img
                  src="./../assets/images/payento-icon.svg"
                  alt="payento-icon"
              /></a>
            </li>
            <li>
              <a href="#"
                ><img src="./../assets/images/logo-normal.svg" alt="logo-normal"
              /></a>
            </li>
            <li>
              <a href="#"
                ><img src="./../assets/images/asset-1.svg" alt="asset-1"
              /></a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style lang="scss" scoped>
@import "./../assets/css/breakpoints.scss";

.header {
  background: url(./../assets/images/header-bg-img.png) no-repeat center;
  background-size: cover;
  width: 100%;
  height: 894px;

  .header-wrap {
    width: 77%;
    margin: 0 auto;
    padding-top: 38px;

    .header-nav-links {
      text-transform: uppercase;
      margin-bottom: 120px;
      a {
        font-weight: 500;
        font-size: 14px;
        letter-spacing: 1.31px;
        display: inline;
      }
      ul {
        display: inline;
        li {
          display: inline;
          margin-right: 60px;
          a {
            color: #220f3e;

            &:hover {
              color: #ff9e08;
            }
          }
        }
      }
      .home-logo {
        display: inline-block;
        height: 44px;
      }
      .contact-us {
        display: inline-block;
        text-align: center;
        padding: 14px 35px;
        background-color: #ff9e08;
        color: #fff;

        &:hover {
          color: #220f3e;
        }
      }

      &::after {
        content: "";
        display: table;
        clear: both;
      }
    }

    .header-welcome {
      display: inline;
      padding: 6px 8px;
      font-weight: 500;
      font-size: 12px;
      color: #220f3e;
      background-color: #fff;
      border-radius: 13px;
      box-shadow: 0 2px 4px 0 rgba(133, 143, 175, 0.1);
      span {
        text-transform: capitalize;
        font-weight: 500;
        font-size: 12px;
        color: #fff;
        border-radius: 13px;
        background-color: #ff9e08;
        padding: 2px 8px;
        margin-right: 8px;
      }
    }

    .header-big-text {
      font-family: "Oswald", sans-serif;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
      font-size: 80px;
      line-height: 90px;
      font-weight: 700;
      color: #220f3e;
      text-transform: uppercase;
      width: 50%;
      margin-top: 16px;
    }

    .header-line-gradient {
      width: 165px;
      height: 4px;
      background: #bb00c4; /* Old browsers */
      background: -moz-linear-gradient(
        left,
        #bb00c4 0%,
        #2989d8 65%,
        #00e3f9 100%
      ); /* FF3.6-15 */
      background: -webkit-linear-gradient(
        left,
        #bb00c4 0%,
        #2989d8 65%,
        #00e3f9 100%
      ); /* Chrome10-25,Safari5.1-6 */
      background: linear-gradient(
        to right,
        #bb00c4 0%,
        #2989d8 65%,
        #00e3f9 100%
      ); /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
      filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#bb00c4', endColorstr='#00e3f9',GradientType=1 ); /* IE6-9 */
      margin: 40px 0;
    }

    .header-msg {
      width: 38%;
      text-align: left;
      p {
        font-weight: 400;
        font-size: 18px;
        line-height: 28px;
        color: #303030;
      }
    }

    .icons-bar {
      display: none;
      width: 100%;
      border-radius: 8px;
      box-shadow: 14px 20px 54px 0 rgba(133, 143, 175, 0.1);
      background-color: #ffffff;
      text-align: center;
      padding: 40px 0;
      position: relative;
      bottom: -232px;
      ul {
        li {
          display: inline-block;

          &:nth-child(even) {
            margin: 0 124px;
          }
          &:nth-child(4),
          &:last-child {
            position: relative;
            top: -7px;
          }

          a {
            display: inline-block;
          }
        }
      }

      @include lg {
        display: block;
      }
    }
  }
}
</style>
