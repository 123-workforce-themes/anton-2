<template>
  <main id="tab-skills">
    <div>
      <b-tabs content-class="mt-3">
        <b-tab title="Programming Languages" active>
          <skill-loader
            :background="'#ffffff'"
            :width="Number(80)"
          >
          <img src="@/assets/img/html5.svg" alt="" class="prog-img">
          </skill-loader>
          <skill-loader
            :background="'#ffffff'"
            :width="Number(30)"
          >
          <img src="@/assets/img/php.svg" alt="" class="prog-img">
          </skill-loader>
          <skill-loader
            :background="'#ffffff'"
            :width="Number(95)"
          >
          <img src="@/assets/img/css3.svg" alt="" class="prog-img">
          </skill-loader>
          <skill-loader
            :background="'#ffffff'"
            :width="Number(50)"
          >
          <img src="@/assets/img/js.svg" alt="" class="prog-img">
          </skill-loader>
        </b-tab>
        <b-tab title="Frameworks/ Databases">
        </b-tab>
        <b-tab title="Design Skills">
        </b-tab>
        <b-tab title="Software">
        </b-tab>
      </b-tabs>
    </div>
  </main>
</template>

<script>
import SkillLoader from '@/components/SkillLoader.vue'

export default {
  components: {
    SkillLoader
  }
}
</script>

<style>
.nav {
  justify-content: center;
  border-bottom: 1px solid rgba(255, 255, 255, 0.12);
  width: 65%;
  margin: auto;
}

.nav-tabs .nav-link {
  border: none;
}

.nav-tabs .nav-link.active, .nav-tabs .nav-item.show .nav-link {
  color: #ffffff !important;
  border: none;
  background: transparent;
  opacity: 1;
}

a {
  color: rgba(255, 255, 255, 0.6);
  opacity: 0.5;
}

a:hover{
  color: rgba(255, 255, 255, 0.6);
  opacity: 0.5;
}

a:active,
a:focus
{
  box-shadow: none;
  outline: none;
}

.prog-img {
  width: 3rem;
}

@media (min-width: 768px) and (max-width: 991.98px) {
  .nav {
    width: 100%;
  }
}

</style>