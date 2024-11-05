<script setup lang="ts">
import { defineProps } from "vue";
import { Button } from "~/components/ui/button";
import {
  Card,
  CardHeader,
  CardTitle,
  CardDescription,
} from "@/components/ui/card";
import { MoveRight } from "lucide-vue-next";

const props = defineProps({
  iconSrc: {
    type: String,
    required: true,
  },
  title: {
    type: String,
    required: true,
  },
  description: {
    type: String,
    required: true,
  },
  buttonText: {
    type: String,
    required: true,
  },
  imageSrc: {
    type: String,
    required: true,
  },
});
</script>
<template>
  <Card class="w-[350px]">
    <CardHeader>
      <div class="flex items-start">
        <img src="@/assets/img/iconcat.png" alt="icon" >
        <CardTitle class="pt-6 font-mochi text-txtpurple">{{
          title
        }}</CardTitle>
      </div>
      <CardDescription class="text-black font-poppins">
        {{ description }}
      </CardDescription>
    </CardHeader>
    <div class="flex justify-between">
      <Button variant="ghost" class="mt-16 ml-4 font-poppins">
        {{ buttonText }} <MoveRight />
      </Button>
      <img src="@/assets/img/cap.png" alt="cap" >
    </div>
  </Card>
</template>


<!-- <template>
    <div class="px-2">
        <Card class="w-[350px]">
          <CardHeader >
            <div class="flex items-start">
              <img src="@/assets/img/iconcat.png" alt="icon cat" />
              <CardTitle class="pt-6 font-mochi text-txtpurple">Dokter Hewan</CardTitle>
            </div>
            
            <CardDescription class="text-black"
                >Layanan kesehatan hewan peliharaan yang profesional dan terpercaya.</CardDescription
            >
          </CardHeader>
          <div class="flex justify-between">
            <Button variant="ghost" class="mt-8 ml-4">Dapatkan Layanan <MoveRight /></Button>
            <img class="" src="@/assets/img/cap.png" alt="cap" />
          </div>
        </Card>
      </div>
</template> -->

