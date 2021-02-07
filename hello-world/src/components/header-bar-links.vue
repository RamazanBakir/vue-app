<template>
  <div class="navbar-menu">
    <div class="navbar-end">
      <div class="navbar-item">
        <div class="buttons">
          <a
              :href="github"
              target="_blank"
              rel="noopener noreferrer"
          >
            <i class="fab fa-github fa-2x" aria-hidden="true"></i>
          </a>
          <!-- href tagında (:) kullandık bu bir kısaltmadır ve içinde olan variable'da
          export tarafında belirtilmiştir. -->
          <a
              v-bind:href="twitter"
              target="_blank"
              rel="noopener noreferrer"
          >
            <i class="fab fa-twitter fa-2x" aria-hidden="true"></i>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name : 'HeaderBarLinks',
  data() {
    return {
      github: 'https://github.com/RamazanBakir/',
      twitter: 'https://twitter.com/',
    };
  },
}
</script>
