<template>
  <div class="content-container">
    <WelcomeItem>
      <template #icon>
        <DocumentationIcon class="icon-style"/>
      </template>
      <template #heading>
        <h2>Documentation</h2>
      </template>
      <p>
        Vue’s
        <a href="https://vuejs.org/" target="_blank" rel="noopener">official documentation</a>
        provides you with semua informasi yang perlu Anda ketahui untuk memulai.
      </p>
    </WelcomeItem>

    <WelcomeItem>
      <template #icon>
        <ToolingIcon class="icon-style"/>
      </template>
      <template #heading>
        <h2>Tooling</h2>
      </template>
      <p>
        Project ini disajikan dan dibundel dengan
        <a href="https://vitejs.dev/guide/features.html" target="_blank" rel="noopener">Vite</a>. 
        Setup IDE yang direkomendasikan adalah
        <a href="https://code.visualstudio.com/" target="_blank" rel="noopener">VSCode</a> + 
        <a href="https://github.com/johnsoncodehk/volar" target="_blank" rel="noopener">Volar</a>. 
        Jika Anda perlu menguji komponen dan halaman web, periksa
        <a href="https://www.cypress.io/" target="_blank" rel="noopener">Cypress</a> dan
        <a href="https://on.cypress.io/component" target="_blank" rel="noopener">Cypress Component Testing</a>.
        <br/>
        Instruksi lebih lanjut tersedia di <code>README.md</code>.
      </p>
    </WelcomeItem>

    <WelcomeItem>
      <template #icon>
        <EcosystemIcon class="icon-style"/>
      </template>
      <template #heading>
        <h2>Ecosystem</h2>
      </template>
      <p>
        Dapatkan alat dan pustaka resmi untuk proyek Anda: 
        <a href="https://pinia.vuejs.org/" target="_blank" rel="noopener">Pinia</a>, 
        <a href="https://router.vuejs.org/" target="_blank" rel="noopener">Vue Router</a>, 
        <a href="https://test-utils.vuejs.org/" target="_blank" rel="noopener">Vue Test Utils</a>, dan
        <a href="https://github.com/vuejs/devtools" target="_blank" rel="noopener">Vue Dev Tools</a>. 
        Jika Anda membutuhkan sumber daya lebih lanjut, kami menyarankan untuk mengunjungi 
        <a href="https://github.com/vuejs/awesome-vue" target="_blank" rel="noopener">Awesome Vue</a>.
      </p>
    </WelcomeItem>

    <WelcomeItem>
      <template #icon>
        <CommunityIcon class="icon-style"/>
      </template>
      <template #heading>
        <h2>Community</h2>
      </template>
      <p>
        Terjebak? Tanyakan pertanyaan Anda di
        <a href="https://chat.vuejs.org" target="_blank" rel="noopener">Vue Land</a>, server Discord resmi kami, atau
        <a href="https://stackoverflow.com/questions/tagged/vue.js" target="_blank" rel="noopener">StackOverflow</a>. 
        Jangan lupa untuk berlangganan
        <a href="https://news.vuejs.org" target="_blank" rel="noopener">mailing list kami</a> dan ikuti
        akun twitter resmi
        <a href="https://twitter.com/vuejs" target="_blank" rel="noopener">@vuejs</a> untuk berita terbaru di dunia Vue.
      </p>
    </WelcomeItem>

    <WelcomeItem>
      <template #icon>
        <SupportIcon class="icon-style"/>
      </template>
      <template #heading>
        <h2>Support Vue</h2>
      </template>
      <p>
        Sebagai proyek independen, Vue bergantung pada dukungan komunitas untuk keberlanjutannya. Anda dapat membantu
        kami dengan
        <a href="https://vuejs.org/sponsor/" target="_blank" rel="noopener">menjadi sponsor</a>.
      </p>
    </WelcomeItem>
  </div>
</template>

<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<style>
  .content-container {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    padding: 20px;
    max-width: 1200px;
    margin: 0 auto;
  }

  .icon-style {
    width: 40px;
    height: 40px;
  }

  h2 {
    margin-bottom: 10px;
    color: #333;
  }

  p {
    font-size: 16px;
    color: #666;
    line-height: 1.5;
  }
</style>
