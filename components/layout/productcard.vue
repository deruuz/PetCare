<script setup lang="ts">
import { defineProps } from 'vue';
import { Button } from '~/components/ui/button';
import { Card, CardHeader, CardTitle } from '@/components/ui/card';
import { Star, MoveRight } from 'lucide-vue-next';

const props = defineProps({
  iconSrc: {
    type: String,
    required: true,
  },
  title: {
    type: String,
    required: true,
  },
  buttonText: {
    type: String,
    required: true,
  },
});
</script>

<template>
    <Card class="w-[350px] my-5">
      <div class="flex items-center">
        <div class="w-64">
          <div class="flex justify-center items-center w-full h-full">
            <img src="@/assets/img/food.png" :alt="title" class="object-scale-down w-full h-full" >
          </div>
        </div>
        <CardHeader>
          <CardTitle class="font-poppins text-lg">{{ title }}</CardTitle>
          <div class="flex text-txtgreen py-2">
            <Star v-for="i in 5" :key="i" class="py-1" />
          </div>
          <Button variant="ghost" class="font-poppins mt-8 ml-4 place-self-end">{{ buttonText }} <MoveRight /></Button>
        </CardHeader>
      </div>
    </Card>
  </template>
  

  
<!-- <template>
  <Card class="w-[350px]">
    <div class="flex item-center">
      <div class="w-64">
        <div class="flex justify-center items-center w-full h-full">
          <img
            src="@/assets/img/food.png"
            alt="food"
            class="object-scale-down w-full h-full"
          />
        </div>
      </div>
      <CardHeader>
        <CardTitle>Pedigree Pouch Makanan Basah </CardTitle>
        <div class="flex text-txtgreen py-2">
          <Star class="py-1" /><Star class="py-1" /><Star
            class="py-1"
          /><Star class="py-1" /><Star class="py-1" />
        </div>
        <Button variant="ghost" class="mt-8 ml-4 place-self-end"
          >Cek Sekarang <MoveRight
        /></Button>
      </CardHeader>
    </div>
  </Card>
</template> -->
