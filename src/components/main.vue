<template>
  <div>
    <div class="main">
      <modal name="new-sub"> thanks for the subscribe, {{ emailsub }}! </modal>
      <modal name="show-message">
        Hello {{ name }} with email address {{ email }}! You sent us the
        following message: {{ message }}</modal
      >
      <div class="main-wrap-1">
        <div class="content-service fine-line">
          <div class="head-grp">
            <div class="title">our services</div>
            <div class="sub">
              Say something about our services will goes here
            </div>
          </div>
          <div class="thumb-grid">
            <a href="#" class="thumbs">
              <img
                src="./../assets/images/001-interface.svg"
                alt="001-interface"
              />
              <div class="title">Enterprise Software</div>
              <p class="desc">
                We will work with you to design, develop and implement a
                customized Enterprise Software Solution based on your needs and
                goals.
              </p>
            </a>
            <a href="#" class="thumbs">
              <img
                src="./../assets/images/002-smartphone.svg"
                alt="002-smartphone"
              />
              <div class="title">Mobile Apps</div>
              <p class="desc">
                Our development team helps you to achieve your goals by
                designing & building custom mobile apps.
              </p>
            </a>
            <a href="#" class="thumbs">
              <img
                src="./../assets/images/003-computer.svg"
                alt="003-computer"
              />
              <div class="title">E-commerce Website</div>
              <p class="desc">
                We build intelligent digital solutions & shopping experiences to
                meet ambitious sales goals for e-commerce businesses.
              </p>
            </a>
            <a href="#" class="thumbs">
              <img src="./../assets/images/004-tablet.svg" alt="004-tablet" />
              <div class="title">Web Development</div>
              <p class="desc">
                We build web apps or work together with your development team to
                create a fully responsive website that stands out.
              </p>
            </a>
          </div>
        </div>
      </div>
      <div class="main-wrap-2">
        <div class="content-coverage fine-line">
          <div class="head-grp">
            <div class="title">We’ve Got You Covered</div>
            <div class="sub">
              <p>
                We’ve combined our technical expertise and proven knowledge of
                latest trends by developing solutions with a better
                user-experience and measurable results for all products- new or
                existing. If you’re looking for solutions for email, we’re a
                one-stop-shop- from delivery service to reputation management.
              </p>
              <p>
                Address : 8th Flr, Skyrise 3, Jose Ma. Del Mar St, Cebu Asiatown
                IT Park, Cebu City
              </p>
            </div>
          </div>
          <div class="info-grp">
            <div class="input-fields">
              <form action="localhost">
                <label for="name">Your name</label>
                <input
                  type="text"
                  id="name"
                  name="name"
                  value="Robert Stark"
                  v-model="name"
                />
                <label for="email">Your Email</label>
                <input
                  type="email"
                  id="email"
                  name="email"
                  placeholder="stark@robert.com"
                  v-model="email"
                />
                <label for="message">Your Message</label>
                <textarea id="message" name="message" v-model="message">
                    Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. : Not active</textarea
                >
                <vue-recaptcha
                  sitekey="6LeyP_sUAAAAADDj5AwrsGqJ00We1RDGPev22DUL"
                  :loadRecaptchaScript="true"
                ></vue-recaptcha>
                <input
                  type="submit"
                  class="form-contact-us"
                  value="CONTACT US"
                  @click="showMessage"
                />
              </form>
            </div>
            <div class="map-holder">
              <iframe
                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1962.5776576845699!2d123.90610179290525!3d10.329452748740641!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x33a999221bba9a59%3A0x7508c4680cd2ed83!2sSkyrise%203!5e0!3m2!1sen!2sph!4v1590222190849!5m2!1sen!2sph"
                width="500"
                height="550"
                frameborder="0"
                style="border:0;"
                allowfullscreen=""
                aria-hidden="false"
                tabindex="0"
              ></iframe>
            </div>
          </div>
        </div>
      </div>
      <div class="main-wrap-3">
        <div class="content-team fine-line">
          <div class="head-grp">
            <div class="title">Meet out team in moebius</div>
            <div class="sub">
              <p>
                Say something about team member will goes here
              </p>
            </div>
          </div>
          <div class="thumbs-gallery">
            <div class="first-row">
              <div class="thumbnail">
                <img src="./../assets/images/rectangle.png" alt="rectangle" />
                <p class="name">Walter Bowers</p>
                <p class="title">HR Manager</p>
              </div>
              <div class="thumbnail">
                <img
                  src="./../assets/images/rectangle-copy-7-1.png"
                  alt="rectangle-copy-7-1"
                />
                <p class="name">Joel Underwood</p>
                <p class="title">Data Entry</p>
              </div>
              <div class="thumbnail">
                <img
                  src="./../assets/images/rectangle-copy-7-2.png"
                  alt="rectangle-copy-7-2"
                />
                <p class="name">Edward Thompson</p>
                <p class="title">Chief Information Officer</p>
              </div>
              <div class="thumbnail">
                <img
                  src="./../assets/images/rectangle-copy-7-3.png"
                  alt="rectangle-7-3"
                />
                <p class="name">Lillie Schwartz</p>
                <p class="title">Technical Specialist</p>
              </div>
            </div>
            <div class="second-row">
              <div class="thumbnail">
                <img
                  src="./../assets/images/rectangle-copy-9.png"
                  alt="rectangle-copy-9"
                />
                <p class="name">Ray Newman</p>
                <p class="title">Web Developer</p>
              </div>
              <div class="thumbnail">
                <img
                  src="./../assets/images/rectangle-copy-11.png"
                  alt="rectangle-copy-11"
                />
                <p class="name">Ronald Vasquez</p>
                <p class="title">Web Developer</p>
              </div>
              <div class="thumbnail">
                <img
                  src="./../assets/images/rectangle-copy-13.png"
                  alt="rectangle-copy-13"
                />
                <p class="name">Sallie Santos</p>
                <p class="title">UX Designer & UI Developer</p>
              </div>
              <div class="thumbnail">
                <img
                  src="./../assets/images/rectangle-copy-15.png"
                  alt="rectangle-copy-13"
                />
                <p class="name">Winifred Abbott</p>
                <p class="title">UX Designer & UI Developer</p>
              </div>
            </div>
          </div>
          <div class="subscribe">
            <p>Subscribe For Free Resources</p>
            <form action="localhost">
              <input
                type="email"
                id="email-sub"
                name="email-sub"
                placeholder="stark@robert.com"
                v-model="emailsub"
              />
              <input
                type="submit"
                class="subscribe-btn"
                value="subscribe"
                @click="showSub"
              />
            </form>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import VueRecaptcha from "vue-recaptcha";

export default {
  name: "Main",
  components: {
    VueRecaptcha,
  },
  data() {
    return {
      name: "Robert Stark",
      email: "stark@robert.com",
      message:
        "Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. : Not active",
      emailsub: "",
    };
  },
  methods: {
    showSub(event) {
      if (event) {
        event.preventDefault();
      }
      this.$modal.show("new-sub");
    },
    hideSub() {
      this.$modal.hide("new-sub");
    },
    showMessage(event) {
      if (event) {
        event.preventDefault();
      }
      this.$modal.show("show-message");
    },
  },
};
</script>

<style lang="scss" scoped>
@import "./../assets/css/breakpoints.scss";

.main {
  padding-bottom: 80px;
  .main-wrap-1 {
    background: none;

    @include lg {
      background: url(./../assets/images/shutterstock-741473680.png) no-repeat;
      background-size: 43%;
      background-position-y: 222px;
    }

    .content-service {
      width: 77%;
      margin: 0 auto;
      margin-top: 80px;

      @include lg {
        margin-top: 133px;
      }

      .head-grp {
        text-align: center;
        margin-bottom: 60px;

        .title {
          font-weight: 500;
          font-size: 30px;
          letter-spacing: 2.8px;
          color: #220f3e;
          text-transform: uppercase;
        }
        .sub {
          font-weight: 400;
          font-size: 18px;
          line-height: 28px;
          color: #8b8b8b;
          margin-top: 24px;
        }
      }
      .thumb-grid {
        @include lg {
          float: right;
          width: 59%;
        }

        .thumbs {
          text-align: left;
          width: 38%;
          height: 244px;
          border-radius: 8px;
          border: solid 1px rgba(133, 143, 175, 0.2);
          background-color: #ffffff;
          padding: 19px;
          float: left;
          margin-left: 20px;

          @include lg {
            width: 40%;
          }

          .title {
            font-weight: 500;
            font-size: 20px;
            color: #2c2c2c;
            margin-top: 32px;
            margin-bottom: 16px;
          }

          &:hover {
            .title {
              color: #ff9e08;
            }
          }
          .desc {
            font-weight: 400;
            font-size: 16px;
            color: #8b8b8b;
          }

          &:first-child,
          &:nth-child(2) {
            margin-bottom: 20px;
          }
        }

        &::after {
          content: "";
          display: table;
          clear: both;
        }
      }

      &::after {
        content: "";
        display: table;
        clear: both;
      }
    }
  }
  .main-wrap-2 {
    .content-coverage {
      width: 77%;
      margin: 0 auto;
      margin-top: 80px;

      .head-grp {
        text-align: center;
        margin-bottom: 60px;

        .title {
          font-weight: 500;
          font-size: 30px;
          letter-spacing: 2.8px;
          color: #220f3e;
          text-transform: uppercase;
        }
        .sub {
          font-weight: 400;
          font-size: 18px;
          line-height: 28px;
          color: #8b8b8b;
          margin-top: 24px;

          p {
            &:first-child {
              margin-bottom: 46px;
            }
          }
        }
      }

      .info-grp {
        position: relative;

        .input-fields {
          border-radius: 8px;
          box-shadow: 14px 20px 54px 0 rgba(133, 143, 175, 0.1);
          background-color: #ffffff;
          width: 96%;
          padding-top: 60px;
          padding-bottom: 60px;
          padding-left: 30px;
          margin-bottom: 24px;

          @include lg {
            border-radius: 8px;
            box-shadow: 14px 20px 54px 0 rgba(133, 143, 175, 0.1);
            background-color: #ffffff;
            width: 80%;
            padding-top: 60px;
            padding-bottom: 90px;
            padding-left: 160px;
            margin-left: -160px;
          }

          form {
            label {
              font-weight: 500;
              font-size: 18px;
              color: #220f3e;
              display: block;
            }
            input,
            textarea {
              font-weight: 400;
              font-size: 18px;
              color: #303030;
              display: block;
              outline: 0;
              border-width: 0 0 1px;
              border-color: #f4f4fa;
              width: 60%;

              &:focus {
                border-color: #ff9e08;
              }
            }
            #name {
              padding: 16px 0;
              margin-bottom: 20px;
            }
            #email {
              padding-top: 27px;
              margin-bottom: 27px;
            }
            #message {
              padding-top: 27px;
              resize: both;
              margin-bottom: 40px;
              width: 60%;
              height: 110px;
              max-width: 60%;
              max-height: 110px;
            }
            #message + div {
              float: left;
            }
            ::-webkit-input-placeholder {
              /* Edge */
              font-size: 18px;
              font-weight: 400;
              color: #8b8b8b;
            }

            :-ms-input-placeholder {
              /* Internet Explorer 10-11 */
              font-size: 18px;
              font-weight: 400;
              color: #8b8b8b;
            }

            ::placeholder {
              font-size: 18px;
              font-weight: 400;
              color: #8b8b8b;
            }
            .form-contact-us {
              font-weight: 500;
              font-size: 14px;
              letter-spacing: 1.31px;
              color: #fff;
              border-radius: 4px;
              background-color: #ff9e08;
              padding: 14px 35px;
              float: left;
              margin-left: 30px;
              border-width: 0;
              cursor: pointer;
              width: auto;
            }

            &::after {
              content: "";
              display: table;
              clear: both;
            }
          }
        }

        .map-holder {
          width: 100%;
          margin: 0 auto;

          iframe {
            width: 100%;
          }

          @include lg {
            float: right;
            position: absolute;
            top: 30px;
            right: 0;
            width: auto;
            margin: 0;

            iframe {
              width: 500px;
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
  .main-wrap-3 {
    .content-team {
      width: 77%;
      margin: 0 auto;
      margin-top: 80px;

      .head-grp {
        text-align: center;
        margin-bottom: 60px;

        .title {
          font-weight: 500;
          font-size: 30px;
          letter-spacing: 2.8px;
          color: #220f3e;
          text-transform: uppercase;
        }
        .sub {
          font-weight: 400;
          font-size: 18px;
          line-height: 28px;
          color: #8b8b8b;
          margin-top: 24px;
        }
      }

      .thumbs-gallery {
        .first-row {
          margin-bottom: 16px;
        }

        .first-row,
        .second-row {
          .thumbnail {
            display: inline-block;
            width: 98%;
            border-radius: 8px;
            border: solid 1px rgba(133, 143, 175, 0.2);
            background-color: #ffffff;

            @include lg {
              display: inline-block;
              width: 23%;
              border-radius: 8px;
              border: solid 1px rgba(133, 143, 175, 0.2);
              background-color: #ffffff;

              &:hover {
                width: 23.5%;
              }
            }

            img {
              width: 100%;
            }

            .name {
              font-weight: 500;
              font-size: 18px;
              color: #2c2c2c;
              padding-top: 24px;
              padding-left: 32px;
            }

            .title {
              font-weight: 400;
              font-size: 14px;
              color: #8b8b8b;
              padding-left: 32px;
              padding-bottom: 32px;
              margin-top: 16px;
            }

            &:first-child,
            &:nth-child(2),
            &:nth-child(3) {
              margin-bottom: 25px;

              @include lg {
                margin-right: 25px;

                &:hover {
                  margin-right: 18px;
                }
              }
            }

            &:last-child:hover {
              @include lg {
                margin-left: -10px;
              }
            }
          }
        }
      }

      .subscribe {
        border-radius: 8px;
        background-color: #ffffff;
        padding: 48px;
        margin-top: 80px;

        p {
          font-weight: 500;
          font-size: 30px;
          letter-spacing: 2.8px;
          color: #220f3e;
          text-transform: uppercase;
        }

        form {
          input {
            font-weight: 400;
            font-size: 18px;
            color: #303030;
            display: inline-block;
            outline: 0;
            border-width: 0 0 1px;
            border-color: #f4f4fa;
            width: 44%;

            &:focus {
              border-color: #ff9e08;
            }
          }

          #email-sub {
            margin-top: 32px;
            padding-bottom: 10px;
          }

          ::-webkit-input-placeholder {
            /* Edge */
            font-size: 18px;
            font-weight: 400;
            color: #8b8b8b;
          }

          :-ms-input-placeholder {
            /* Internet Explorer 10-11 */
            font-size: 18px;
            font-weight: 400;
            color: #8b8b8b;
          }

          ::placeholder {
            font-size: 18px;
            font-weight: 400;
            color: #8b8b8b;
          }

          .subscribe-btn {
            font-weight: 500;
            font-size: 14px;
            letter-spacing: 1.31px;
            color: #fff;
            border-radius: 4px;
            background-color: #ff9e08;
            padding: 14px 40px;
            float: right;
            border-width: 0;
            cursor: pointer;
            width: auto;
            text-transform: uppercase;
          }

          &:after {
            content: "";
            display: table;
            clear: both;
          }
        }
      }
    }
  }
}
</style>
