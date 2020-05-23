<template>
  <div>
    <div class="footer">
      <div class="footer-bg-overlay">
        <div class="footer-wrap">
          <div class="top">
            <a href="#">
              <img
                src="./../assets/images/moebius-logo-white.svg"
                alt="moebius-logo-white"
              />
            </a>
            <ul>
              <li><a href="#">home</a></li>
              <li><a href="#">service</a></li>
              <li><a href="#">about</a></li>
              <li><a href="#">jobs</a></li>
            </ul>
          </div>
          <div class="bottom">
            <p class="copyright">Copyright&#169; 2020</p>
            <div class="follow-us">
              <span>Follow us</span>
              <ul>
                <li>
                  <a href="#"
                    ><img
                      src="./../assets/images/001-facebook.svg"
                      alt="001-facebook"
                  /></a>
                </li>
                <li>
                  <a href="#"
                    ><img
                      src="./../assets/images/002-twitter.svg"
                      alt="002-twitter"
                  /></a>
                </li>
                <li>
                  <a href="#"
                    ><img
                      src="./../assets/images/003-linkedin.svg"
                      alt="003-linkedin"
                  /></a>
                </li>
                <li>
                  <a href="#"
                    ><img
                      src="./../assets/images/005-instagram.svg"
                      alt="005-instagram"
                  /></a>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style lang="scss" scoped>
.footer {
  background: #ffaf35; /* Old browsers */
  background: -moz-linear-gradient(
    top,
    #ffaf35 0%,
    #ff7c11 67%,
    #ff7d10 100%
  ); /* FF3.6-15 */
  background: -webkit-linear-gradient(
    top,
    #ffaf35 0%,
    #ff7c11 67%,
    #ff7d10 100%
  ); /* Chrome10-25,Safari5.1-6 */
  background: linear-gradient(
    to bottom,
    #ffaf35 0%,
    #ff7c11 67%,
    #ff7d10 100%
  ); /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
  filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#ffaf35', endColorstr='#ff7d10',GradientType=0 ); /* IE6-9 */

  .footer-bg-overlay {
    background-image: url(./../assets/images/group-13.svg);
    background-repeat: no-repeat;
    background-position: 128% 100%;
    padding: 40px 0;

    .footer-wrap {
      width: 77%;
      margin: 0 auto;

      .top {
        a {
          display: inline-block;

          img {
            float: left;
          }
        }
        ul {
          float: right;
          margin-top: 14px;

          li {
            display: inline;

            &:not(:nth-child(4)) {
              margin-right: 60px;
            }

            a {
              font-weight: 500;
              font-size: 14px;
              letter-spacing: 1.31px;
              color: #fff;
              text-transform: uppercase;

              &:hover {
                color: #220f3e;
              }
            }
          }
        }

        &::after {
          content: "";
          display: table;
          clear: both;
        }
      }

      .bottom {
        margin-top: 80px;

        .copyright {
          font-weight: 400;
          font-size: 12px;
          letter-spacing: 1.12px;
          color: #fff;
          display: block;
          float: left;
        }

        .follow-us {
          float: right;

          span {
            display: inline-block;
            font-weight: 400;
            font-size: 12px;
            letter-spacing: 1.12px;
            color: #fff;
            margin-right: 16px;
            position: relative;
            top: -4px;
          }

          ul {
            display: inline;

            li {
              display: inline;

              &:not(:nth-child(4)) {
                margin-right: 8px;
              }

              a {
                display: inline-block;

                &:hover {
                  img {
                    width: 22px;
                  }
                }
              }
            }
          }
        }

        &::after {
          content: "";
          display: table;
          clear: both;
        }
      }
    }
  }
}
</style>
