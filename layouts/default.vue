<template>
  <div>
    <NavBar brand="Jonas Holmström" />

    <div>
      <nuxt />
    </div>

    <footer class="footer">
      <div class="container">
        <div class="columns is-multiline">
          <div class="column is-7">
            <p>
              Jag är en webbutvecklare med mycket teknisk kunskap och är bosatt i Skåne.<br>
              Välkommen att kontakta mig om du behöver hjälp eller råd med något webbrelaterat!
            </p>
          </div>
          <div class="column is-5">
            <ul>
              <li>
                <span class="icon">
                  <i class="fa fa-envelope-o" aria-hidden="true" />
                </span>
                <a href="mailto:jonas@holmstrom.me">jonas@holmstrom.me</a>
              </li>
              <li>
                <span class="icon">
                  <i class="fa fa-phone" aria-hidden="true" />
                </span>
                0735-584567
              </li>
              <li>
                <span class="icon">
                  <i class="fa fa-twitter" aria-hidden="true" />
                </span>
                <a href="https://twitter.com/notnotjonas" target="_blank">Twitter</a>
              </li>
              <li>
                <span class="icon">
                  <i class="fa fa-linkedin" aria-hidden="true" />
                </span>
                <a href="https://www.linkedin.com/in/jonas-holmstr%C3%B6m-69b21a81/" target="_blank">LinkedIn</a>
              </li>
              <li>
                <span class="icon">
                  <i class="fa fa-github" aria-hidden="true" />
                </span>
                <a href="https://github.com/Foof" target="_blank">Github</a>
              </li>
            </ul>
          </div>
          <div class="column">
            <p><strong>&copy; {{ (new Date()).getFullYear() }} – Jonas Holmström</strong></p>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
import NavBar from '../components/NavBar'

export default {
  components: {
    NavBar
  }
}
</script>
