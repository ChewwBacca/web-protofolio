<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>


<template>
  <div class="row">
    <div class="col-text">
      <WelcomeItem>
        <template #icon>
          <DocumentationIcon />
        </template>
        <template #heading>BIODATA DIRI </template>

        Perkenalkan nama saya Muh. Azizurrohman, Biasa dipanggil Aziz. Saya lulusan dari SMAN 1 LUBUK BATU JAYA
        dan saat ini sedang menenempuh pendidikan tinggi di Universitas Islam Riau dengan mengambil Program Studi
        Teknik Informatika.

      </WelcomeItem>

      <WelcomeItem>
        <template #icon>
          <ToolingIcon />
        </template>
        <template #heading>SKILL</template>

        - Teamwork<br>
        - Mampu berpikir secara rasional dan tidak individualis
      </WelcomeItem>

      <WelcomeItem>
        <template #icon>
        <SupportIcon />
        </template>
        <template #heading>KEMAMPUAN</template>

        - Kejujuran<br>
        - Kemampuan beradaptasi<br>
        - Bisa berbahasa Inggris
      </WelcomeItem>

      <WelcomeItem>
        <template #icon>
          <EcosystemIcon />
        </template>
        <template #heading>PENGALAMAN</template>
        - Mengikuti Marathon 5 km di lapangan terbang Roesmin Noerjadin.<br>
        - Mengikuti lari 10 km Virtual<br>
        - Menang lomba cosplay pahlawan saat class meeting SMP
      </WelcomeItem>
    </div>
    <div class="col-image">
      <img src="../assets/1.png" alt="Large Image" class="large-image" />
    </div>
  </div>
</template>


<style scoped>
  .row {
    display: flex;
  }

  .col-text {
    flex: 1;
    display: flex;
    flex-direction: column;
    justify-content: center;
    margin-right: auto;
  }

  .col-image {
    flex: 0 0 auto;
    width: 300px;
  }


  .col-text p {
    white-space: nowrap;
  }

  .col-text .welcome-item {
    margin-bottom: 10px;
  }

  .large-image {
    width: 200%;
    margin-top: 100%;
    margin-left: 100%;
  }
</style>
