<template>
  <div class="bg-white py-24 sm:py-32">
    <div class="mx-auto grid max-w-7xl gap-x-8 gap-y-20 px-6 lg:px-8 xl:grid-cols-3">
      <div class="max-w-2xl">
        <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">STRUKTUR PIMPINAN CABANG MUHAMMADIYAH (PCM) BATAM KOTA</h2>
        <p class="mt-6 text-lg leading-8 text-gray-600">Libero fames augue nisl porttitor nisi, quis. Id ac elit odio vitae elementum enim vitae ullamcorper suspendisse.</p>
      </div>
      <ul role="list" class="grid gap-x-8 gap-y-12 sm:grid-cols-2 sm:gap-y-16 xl:col-span-2">
        <li v-for="person in people" :key="person.name">
          <div class="flex items-center gap-x-6">
            <img class="h-20 w-20 rounded-full" :src="person.imageUrl" alt="" />
            <div>
              <h3 class="text-base font-semibold leading-7 tracking-tight text-gray-900">{{ person.name }}</h3>
              <p class="text-sm font-semibold leading-6 text-indigo-600">{{ person.role }}</p>
            </div>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup>
const people = [
  {
    name: 'Ustaz Subkhi Al-Bughury',
    role: 'Ketua Pimpinan Cabang Batam Kota',
    imageUrl:
      'https://3.bp.blogspot.com/-J59lvVFtt0I/WSgTxM_upNI/AAAAAAAABuA/Gmljji2gw2kEYIXKuBAFnxit-DcU3NfaQCLcB/s1600/profil%2Bbiodata%2Bustadz%2Bsubki%2Bal%2Bbughury.jpg',
  },
  {
  name: 'Ustaz Subkhi Al-Bughury',
    role: 'Ketua Pimpinan Cabang Batam Kota',
    imageUrl:
      'https://3.bp.blogspot.com/-J59lvVFtt0I/WSgTxM_upNI/AAAAAAAABuA/Gmljji2gw2kEYIXKuBAFnxit-DcU3NfaQCLcB/s1600/profil%2Bbiodata%2Bustadz%2Bsubki%2Bal%2Bbughury.jpg',
  },
  {
    name: 'Ustaz Subkhi Al-Bughury',
    role: 'Ketua Pimpinan Cabang Batam Kota',
    imageUrl:
      'https://3.bp.blogspot.com/-J59lvVFtt0I/WSgTxM_upNI/AAAAAAAABuA/Gmljji2gw2kEYIXKuBAFnxit-DcU3NfaQCLcB/s1600/profil%2Bbiodata%2Bustadz%2Bsubki%2Bal%2Bbughury.jpg',
  },
]
</script>