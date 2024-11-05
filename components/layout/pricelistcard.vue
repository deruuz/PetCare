<script setup lang="ts">
import { defineProps } from 'vue';
import { Button } from '~/components/ui/button';
import { Card, CardHeader, CardTitle } from '@/components/ui/card';
import { CircleCheck } from 'lucide-vue-next';

const props = defineProps({
  title: {
    type: String,
    required: true,
  },
  price: {
    type: String,
    required: true,
  },
  services: {
    type: Array,
    required: true,
  },
  buttonText: {
    type: String,
    required: true,
  },
});
</script>

<template>
    <Card class="w-[350px]">
      <CardHeader>
        <CardTitle class="flex justify-center font-mochi text-txtpurple">
          {{ title }}
        </CardTitle>
      </CardHeader>
      <div>
        <div class="flex justify-center">
          <Button class="bg-txtgreen px-6 py-6 font-poppins text-2xl" disabled>
            {{ price }}
          </Button>
        </div>
  
        <div class="flex flex-col items-center font-poppins text-txtpurple">
          <Button variant="ghost" class="mt-4" v-for="(service, index) in services" :key="index" disabled>
            <CircleCheck /> {{ service }}
          </Button>
        </div>
        <div class="flex justify-center">
          <Button class="my-8 text-txtgreen font-poppins hover:text-txtgreen" variant="outline">
            {{ buttonText }}
          </Button>
        </div>
      </div>
    </Card>
  </template>
  

<!-- <template>
    <Card class="w-[350px]">
      <CardHeader>
        <CardTitle class="flex justify-center font-mochi text-txtpurple"
          >Regular Groom</CardTitle
        >
      </CardHeader>
      <div>
        <div class="flex justify-center">
          <Button class="bg-txtgreen px-6 py-6 font-poppins text-2xl"
            >Rp. 100.000</Button
          >
        </div>

        <div class="flex flex-col items-center font-poppins text-txtpurple">
          <Button variant="ghost" class="mt-4"
            ><CircleCheck />Dapatkan Layanan
          </Button>
          <Button variant="ghost" class="mt-4">
            <CircleCheck />Dapatkan Layanan
          </Button>
          <Button variant="ghost" class="mt-4">
            <CircleCheck />Dapatkan Layanan
          </Button>
          <Button variant="ghost" class="mt-4">
            <CircleCheck />Dapatkan Layanan
          </Button>
          <Button variant="ghost" class="mt-4"
            ><CircleCheck /> Dapatkan Layanan
          </Button>
          <Button variant="ghost" class="mt-4"
            ><CircleCheck /> Dapatkan Layanan
          </Button>
        </div>
        <div class="flex justify-center">
          <Button
            class="my-8 text-txtgreen font-poppins hover:text-txtgreen"
            variant="outline"
            >Cek Sekarang</Button
          >
        </div>
      </div>
    </Card>
</template> -->