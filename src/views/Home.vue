<template>
  <main id="home" class="overlay">
    <section class="top-section">
      <div class="avatar-container">
        <div class="avatar"></div>
        <div class="user-deets">
          <p>Jennifer lopez</p>
          <span>Web Designer</span>
        </div>
        <div class="icon-container">
          <div class="icon1">
            <img src="@/assets/img/chat.svg" alt="">
          </div>
          <div class="icon2">
            <img src="@/assets/img/audio.svg" alt="">
          </div>
          <div class="icon3">
            <img src="@/assets/img/video.svg" alt="">
          </div>
        </div>
      </div>
      <div class="rate">
        <div class="rate-deets">
          <p class="with-line"><span>$10</span> hourly rate</p>
          <p class="weekly"><span>35 HOURS</span> weekly availability</p>
          <button class="btn btn-sm hire">HIRE ME</button>
        </div>
      </div>
    </section>
    <section class="social-media">
      <div class="social">
        <i class="fab fa-behance"></i>
      </div>
      <div class="social">
        <i class="fab fa-dribbble"></i>
      </div>
      <div class="social">
        <i class="fab fa-pinterest-p"></i>
      </div>
      <div class="social">
        <img src="@/assets/img/instagram.svg" alt="">
      </div>
      <div class="social">
        <i class="fab fa-linkedin-in"></i>
      </div>
    </section>
    <section class="tab-container">
      <div class="tab-header">
        <div>
        <a 
          id="first-tab"
          :class="{ active: isActive('portfolio') }"
          data-toggle="tab"
          role="tab"
          aria-controls="first"
          aria-selected="true"
          @click.prevent="setActive('portfolio', 0)">
          
          <h5 :class="{ active: isActive('portfolio') }">Portfolio</h5>
        </a>
      </div>
      <div>
        <a 
          id="second-tab"
          data-toggle="tab"
          role="tab"
          aria-controls="second"
          aria-selected="true"
          @click.prevent="setActive('skills', 1)">

          <h5 :class="{ active: isActive('skills') }">Skills</h5>
        </a>
      </div>
      <div>
          <a 
            id="third-tab"
            data-toggle="tab"
            role="tab"
            aria-controls="third"
            aria-selected="true"
            @click.prevent="setActive('work', 2)">

            <h5 :class="{ active: isActive('work') }">Work</h5>
          </a>
        </div>
        <div>
          <a 
            id="fourth-tab"
            data-toggle="tab"
            role="tab"
            aria-controls="fourth"
            aria-selected="true"
            @click.prevent="setActive('education', 3)">

            <h5 :class="{ active: isActive('education') }">Education</h5>
          </a>
        </div>
      </div>
      <div id="myTabContent" class="tab-content">
        <div
            id="portfolio"
            class="tab-pane"
            role="tabpanel"
            aria-labelledby="first-tab"
            :class="{ 'active show': isActive('portfolio') }">

            <div class="img-section">
              <div class="col-lg-4 col-md-12 col-sm-12">
                <img src="@/assets/img/tab1.png" alt="">
              </div>
              <div class="col-lg-4 col-md-12 col-sm-12">
                <img src="@/assets/img/tab2.png" alt="">
              </div>
              <div class="col-lg-4 col-md-12 col-sm-12">
                <img src="@/assets/img/tab3.png" alt="">
              </div>
            </div>
          </div>
           <div
            id="skills"
            class="tab-pane"
            role="tabpanel"
            aria-labelledby="second-tab"
            :class="{ 'active show': isActive('skills') }">
            <div class="mobile__tab">
              <tab-component></tab-component>
            </div>
          </div>
          <div
            id="work"
            class="tab-pane"
            role="tabpanel"
            aria-labelledby="third-tab"
            :class="{ 'active show': isActive('work') }">

              <div class="text-container">
                <div class="left-container space">
                  <div class="left-first">
                    <div class="d-flex justify-content-between">
                      <div>
                        <h6 class="big-text">Graphic &amp; web Designer</h6>
                        <p class="pt-5">2018 - 2019</p>
                      </div>
                      <div>
                        <h6 class="sub-heading">Company "React"</h6>
                          <ul class="list-unstyled">
                            <li>
                              - Turning creative concepts into finished websites.
                            </li>
                            <li>
                              - Drawing up detailed website s pecifications.
                            </li>
                            <li>
                              - Building websites that are easy to understand, navigate and use.
                            </li>
                            <li>
                              - Designing sample page layouts.
                            </li>
                            <li>
                              - Ensuring that the website complies with the company’s brand guidelines.
                            </li>
                          </ul>
                      </div>
                    </div>
                  </div>
                  <div class="left-first">
                    <div class="d-flex justify-content-between mt-5">
                      <div>
                        <h6 class="big-text">Graphic &amp; web Designer</h6>
                        <p class="pt-5">2018 - 2019</p>
                      </div>
                      <div>
                        <h6 class="sub-heading">Company "React"</h6>
                          <ul class="list-unstyled">
                            <li>
                              - Turning creative concepts into finished websites.
                            </li>
                            <li>
                              - Drawing up detailed website s pecifications.
                            </li>
                            <li>
                              - Building websites that are easy to understand, navigate and use.
                            </li>
                            <li>
                              - Designing sample page layouts.
                            </li>
                            <li>
                              - Ensuring that the website complies with the company’s brand guidelines.
                            </li>
                          </ul>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="left-container">
                  <div class="left-first">
                    <div class="d-flex justify-content-between">
                      <div>
                        <h6 class="big-text">Graphic &amp; web Designer</h6>
                        <p class="pt-5">2018 - 2019</p>
                      </div>
                      <div>
                        <h6 class="sub-heading">Company "React"</h6>
                          <ul class="list-unstyled">
                            <li>
                              - Turning creative concepts into finished websites.
                            </li>
                            <li>
                              - Drawing up detailed website s pecifications.
                            </li>
                            <li>
                              - Building websites that are easy to understand, navigate and use.
                            </li>
                            <li>
                              - Designing sample page layouts.
                            </li>
                            <li>
                              - Ensuring that the website complies with the company’s brand guidelines.
                            </li>
                          </ul>
                      </div>
                    </div>
                  </div>
                  <div class="left-first">
                    <div class="d-flex justify-content-between mt-5">
                      <div>
                        <h6 class="big-text">Graphic &amp; web Designer</h6>
                        <p class="pt-5">2018 - 2019</p>
                      </div>
                      <div>
                        <h6 class="sub-heading">Company "React"</h6>
                          <ul class="list-unstyled">
                            <li>
                              - Turning creative concepts into finished websites.
                            </li>
                            <li>
                              - Drawing up detailed website s pecifications.
                            </li>
                            <li>
                              - Building websites that are easy to understand, navigate and use.
                            </li>
                            <li>
                              - Designing sample page layouts.
                            </li>
                            <li>
                              - Ensuring that the website complies with the company’s brand guidelines.
                            </li>
                          </ul>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
          </div>

          <div
            id="education"
            class="tab-pane"
            role="tabpanel"
            aria-labelledby="fourth-tab"
            :class="{ 'active show': isActive('education') }">

              <div class="text-container">
                <div class="left-container space">
                  <div class="left-first">
                    <div class="d-flex justify-content-between">
                      <div>
                        <h6 class="big-text">Master in Web Developer</h6>
                        <p class="pt-5">2018 - 2019</p>
                      </div>
                      <div>
                        <h6 class="sub-heading">Envision Media, Inc., Santa Cruz, CA</h6>
                          <ul class="list-unstyled">
                            <li>
                              - Turning creative concepts into finished websites.
                            </li>
                            <li>
                              - Drawing up detailed website s pecifications.
                            </li>
                            <li>
                              - Building websites that are easy to understand, navigate and use.
                            </li>
                            <li>
                              - Designing sample page layouts.
                            </li>
                            <li>
                              - Ensuring that the website complies with the company’s brand guidelines.
                            </li>
                          </ul>
                      </div>
                    </div>
                  </div>
                  <div class="left-first">
                    <div class="d-flex justify-content-between mt-5">
                      <div>
                        <h6 class="big-text">Master in Web Developer</h6>
                        <p class="pt-5">2018 - 2019</p>
                      </div>
                      <div>
                        <h6 class="sub-heading">Envision Media, Inc., Santa Cruz, CA</h6>
                          <ul class="list-unstyled">
                            <li>
                              - Turning creative concepts into finished websites.
                            </li>
                            <li>
                              - Drawing up detailed website s pecifications.
                            </li>
                            <li>
                              - Building websites that are easy to understand, navigate and use.
                            </li>
                            <li>
                              - Designing sample page layouts.
                            </li>
                            <li>
                              - Ensuring that the website complies with the company’s brand guidelines.
                            </li>
                          </ul>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="left-container">
                  <div class="left-first">
                    <div class="d-flex justify-content-between">
                      <div>
                        <h6 class="big-text">Master in Web Developer</h6>
                        <p class="pt-5">2018 - 2019</p>
                      </div>
                      <div>
                        <h6 class="sub-heading">Envision Media, Inc., Santa Cruz, CA</h6>
                          <ul class="list-unstyled">
                            <li>
                              - Turning creative concepts into finished websites.
                            </li>
                            <li>
                              - Drawing up detailed website s pecifications.
                            </li>
                            <li>
                              - Building websites that are easy to understand, navigate and use.
                            </li>
                            <li>
                              - Designing sample page layouts.
                            </li>
                            <li>
                              - Ensuring that the website complies with the company’s brand guidelines.
                            </li>
                          </ul>
                      </div>
                    </div>
                  </div>
                  <div class="left-first">
                    <div class="d-flex justify-content-between mt-5">
                      <div>
                        <h6 class="big-text">Master in Web Developer</h6>
                        <p class="pt-5">2018 - 2019</p>
                      </div>
                      <div>
                        <h6 class="sub-heading">Envision Media, Inc., Santa Cruz, CA</h6>
                          <ul class="list-unstyled">
                            <li>
                              - Turning creative concepts into finished websites.
                            </li>
                            <li>
                              - Drawing up detailed website s pecifications.
                            </li>
                            <li>
                              - Building websites that are easy to understand, navigate and use.
                            </li>
                            <li>
                              - Designing sample page layouts.
                            </li>
                            <li>
                              - Ensuring that the website complies with the company’s brand guidelines.
                            </li>
                          </ul>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
          </div>
      </div>
      <div class="nav-arrows">
        <div>
          <i class="far fa-arrow-alt-circle-left fa-2x pr-3"></i>
        </div>
        <div>
          <i class="far fa-arrow-alt-circle-right fa-2x"></i>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
import TabComponent from '@/components/TabComponent.vue'

export default {
  components: {
    TabComponent
  },
  data() {
    return {
      activeItem: 'portfolio',
      currentLink: 0
    }
  },
  methods: {
    isActive (menuItem) {
      return this.activeItem === menuItem;
    },
   setActive (menuItem, y) {
      this.activeItem = menuItem;
      this.currentLink = y;
    },
    // moveRight() {
    //   if(this.currentLink <= 3) {
    //     this.currentLink + 1
    //     this.activeItem = 'skills'
    //   } else {
    //     this.currentLink = 0
    //   }
    // },
    // moveLeft() {
    //   if(this.currentLink == 3) {
    //     this.currentLink - 1
    //     this.activeItem = 'portfolio'
    //   }
    // }
  }

}
</script>

<style scoped>

.overlay {
  background: rgba(86, 86, 86, 0.9);
  height: 100vh;
  color: #ffffff;
  overflow-y: scroll;
  font-family: 'Raleway', sans-serif;
  padding: 50px 50px 0px 50px;
}

#home .top-section,
#home .top-section .avatar-container,
#home .top-section .icon-container,
#home .top-section .rate
{
  display: flex;
  justify-content: space-between;
}

#home .top-section .avatar-container .avatar {
  width: 6rem;
  height: 6rem;
  border-radius: 50%;
  border: 1px solid #ffffff;
}

#home .top-section .avatar-container .user-deets {
  line-height: 10px;
  padding: 1.4rem;
}

#home .top-section .avatar-container .user-deets p {
  font-size: 24px
}

#home .top-section .avatar-container .user-deets span {
  font-size: 14px;
  font-weight: 300;
}

#home .top-section .avatar-container .icon-container .icon1,
#home .top-section .avatar-container .icon-container .icon2,
#home .top-section .avatar-container .icon-container .icon3
{
  width: 3rem;
  height: 3rem;
  margin: 16px 8px;
  border-radius: 50%;
  border: 1px solid #ffffff;
  display: flex;
  justify-content: center;
  align-items: center
}

#home .top-section .rate .rate-deets {
  display: flex;
  justify-content: space-between;
  align-items: center
}

#home .top-section .rate .rate-deets span {
  font-weight: 600;
  font-size: 18px !important;
}

#home .top-section .rate .rate-deets p {
  font-size: 13px;
}


#home .top-section .rate .rate-deets .with-line {
  border-right: 1px solid #ffffff;
  height: 22px;
  padding-right: 20px;
}

#home .top-section .rate .rate-deets .weekly {
  padding-left: 15px;
}

#home .top-section .rate .rate-deets button {
  border: 1px solid #ffffff;
  color: #ffffff;
  box-sizing: border-box;
  border-radius: 50px;
  width: 140px;
  height: 48px;
  margin-top: -23px;
  margin-left: 17px;
}

#home .top-section .rate .rate-deets button:active,
#home .top-section .rate .rate-deets button:focus
 {
  box-shadow: none;
  outline: none;
}

#home .social-media {
  display: flex;
  justify-content: center;
  align-items: center;
  border-top: 1px solid #737373;
  border-bottom: 1px solid #737373;
  margin: 60px 0px;
  padding: 30px 0px;
}

#home .social-media .social {
  border: 1px solid #ffffff;
  border-radius: 50%;
  width: 48px;
  height: 48px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0px 10px;
}

#home .social-media .social img {
  width: 22px;
}
  
.fab {
  font-size: 22px;
}

#home .tab-container .tab-header {
  display: flex;
  justify-content: center;
  align-items: center;
}

#home .tab-container .tab-header a >>> h5 {
  font-weight: 300;
  padding: 0px 45px;
  cursor: pointer;
}

#home .tab-container .tab-header a .active {
  font-size: 50px;
  font-weight: 300;
}

#home .tab-container .tab-header a .active::after {
  position: absolute;
  border: 1px solid red;
}

#home .tab-container .tab-content {
  padding: 50px 0px;
}

#home .tab-container .img-section {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

#home .tab-container .img-section img {
  width: 100%;
  border-radius: 20px;
}

#home .text-container
 {
  display: flex;
  justify-content: space-between;
  margin: 1rem;
}

#home .text-container .space {
  padding-right: 5rem;
}

#home .text-container .sub-heading {
  font-size: 20px;
  font-weight: 600;
  margin-top: -6px;
}

#home .nav-arrows {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 1rem 0rem;
  cursor: pointer;
}

@media (min-width: 768px) and (max-width: 991.98px) {
  #home .top-section{
   display: flex;
   flex-direction: column;
  }

  #home .top-section .rate {
    padding: 3rem 0rem;
    margin: auto;
  }

  #home .top-section .avatar-container {
    padding: 0rem 3rem;
  }

  #home .tab-container .img-section {
    display: flex;
    flex-direction: column;
  }

  #home .text-container {
    flex-direction: column;
    padding-left: 6rem;
  }

   #home .text-container .left-first {
    padding: 1rem 0rem;
  }
}

@media (min-width: 576px) and (max-width: 767.98px) {

}
</style>