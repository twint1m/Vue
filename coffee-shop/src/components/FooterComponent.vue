<template>
    <footer>
        <div class="container">
          <div class="row">
            <div class="col-lg-6 offset-lg-3">
              <ul class="footer d-flex flex-wrap">
                <li class="footer__item">
                  <router-link :to="links[0].link">
                    <img 
                      :src="require(`@/assets/logo/${links[0].icon}`)"
                      :alt="links[0].icon" />
                  </router-link>
                </li>
                <li class="footer__item">
                  <router-link :to="links[1].link">{{ links[1].text }}</router-link>
                </li>
                <li class="footer__item">
                  <router-link :to="links[2].link">{{ links[2].text }}</router-link>
                </li>
                <li class="footer__item">
                  <router-link :to="links[3].link">{{ links[3].text }}</router-link>
                </li>
              </ul>
            </div>
          </div>
          <img
            class="beanslogo"
            src="@/assets/logo/Beans_logo_dark.svg"
            alt="Beans logo"
          />
        </div>
      </footer>
</template>

<script>
  export default {
    data() {
      return {
        links: [
          {
            id: 0,
            link: '/',
            icon: 'Logo_black.svg'
          },
          {
            id: 1,
            text: 'Our coffee',
            link: '/our-coffee'
          },
          {
            id: 2,
            text: 'For your pleasure',
            link: '/for-your-pleasure'
          },
          {
            id: 3,
            text: 'Contact Us',
            link: '/contact-us'
          }
        ]
      }
    }
  }
</script>