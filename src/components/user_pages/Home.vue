<template>
  <Header></Header>
  <main class="container mx-auto dark:bg-gray-900">
    <section
      class="relative bg-[url('../images/One.jpg')] bg-cover bg-center min-h-[60vh] md:min-h-[80vh] flex items-center justify-center"
    >
      <div class="absolute inset-0 bg-black/50"></div>
      <div class="relative z-10 max-w-2xl text-center text-white px-6">
        <h1 class="text-3xl md:text-5xl font-bold mb-6 leading-tight">
          SAVE THE CHILDREN HELP ALL CHILDREN IN THE WORLD
        </h1>
        <a
          href="https://www.savethechildren.ma/the-waed-network"
          class="inline-block bg-red-700 hover:bg-red-800 text-white font-semibold px-6 py-3 rounded-lg transition-colors"
        >
          The Wa’ed Network
        </a>
      </div>
    </section>

    <!-- مربعات المشاريع مع دعم الوضع الليلي -->
    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8 my-12">
      <div class="bg-white dark:bg-gray-800 rounded-xl shadow-lg border border-gray-200 dark:border-gray-700 flex flex-col overflow-hidden transition-transform duration-300 hover:scale-105 hover:shadow-2xl">
        <img src="/images/L1009660.jpg" alt="Foundation founding" class="w-full h-64 object-cover" />
        <div class="p-6 flex flex-col flex-1 justify-between">
          <h3 class="text-2xl font-bold text-gray-900 dark:text-white mb-4">Our mission</h3>
          <p class="text-gray-600 dark:text-gray-300 mb-6 flex-1">
            SaveTheChildren aims to end all kinds of violence against women in the Arab region. We mobilize women’s influence and participation across all sectors - political, legal and civil activism - to address women’s advancement, security, protection, and participation.
          </p>
          <button class="w-full bg-red-700 hover:bg-red-800 text-white font-semibold px-6 py-3 rounded-lg transition-colors">
            Read More
          </button>
        </div>
      </div>
      <div class="bg-white dark:bg-gray-800 rounded-xl shadow-lg border border-gray-200 dark:border-gray-700 flex flex-col overflow-hidden transition-transform duration-300 hover:scale-105 hover:shadow-2xl">
        <img src="/images/IMG-20190410-WA0001.jpg" alt="Team growth" class="w-full h-64 object-cover" />
        <div class="p-6 flex flex-col flex-1 justify-between">
          <h3 class="text-2xl font-bold text-gray-900 dark:text-white mb-4">Our approach</h3>
          <p class="text-gray-600 dark:text-gray-300 mb-6 flex-1">
            Help children
          </p>
          <button class="w-full bg-red-700 hover:bg-red-800 text-white font-semibold px-6 py-3 rounded-lg transition-colors">
            Read More
          </button>
        </div>
      </div>
      <div class="bg-white dark:bg-gray-800 rounded-xl shadow-lg border border-gray-200 dark:border-gray-700 flex flex-col overflow-hidden transition-transform duration-300 hover:scale-105 hover:shadow-2xl">
        <img src="/images/IMG-20190429-WA0034.jpg" alt="Our priorities" class="w-full h-64 object-cover" />
        <div class="p-6 flex flex-col flex-1 justify-between">
          <h3 class="text-2xl font-bold text-gray-900 dark:text-white mb-4">Our priorities</h3>
          <p class="text-gray-600 dark:text-gray-300 mb-6 flex-1">
            Activists in the SaveTheChildren network work across Africa and the Middle East to dismantle legal frameworks that ingrain inequality, replacing them with modern laws that protect women and girls. SaveTheChildren supports its partners to help them achieve meaningful impact and sustainable results.
          </p>
          <button class="w-full bg-red-700 hover:bg-red-800 text-white font-semibold px-6 py-3 rounded-lg transition-colors">
            Read More
          </button>
        </div>
      </div>
    </div>
  </main>
  <Footer></Footer>
</template>

<script setup>
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';

const toggleDarkMode = () => {
  isDark.value = !isDark.value;
  if (isDark.value) {
    document.documentElement.classList.add('dark'); // يضيف الكلاس إلى <html>
  } else {
    document.documentElement.classList.remove('dark');
  }
};
</script>
