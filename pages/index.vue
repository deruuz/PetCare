<script setup lang="ts">
import navbar from "@/components/layout/navbar.vue";
import Footer from "@/components/layout/footer.vue";
import ServiceCard from "@/components/layout/servicecard.vue";
import ProductCard from "@/components/layout/productcard.vue";
import PriceListCard from "@/components/layout/pricelistcard.vue";

import { Button } from "~/components/ui/button";
import {
  Card,
  CardContent,
  CardDescription,
  CardFooter,
  CardHeader,
  CardTitle,
} from "@/components/ui/card";
import { Input } from "@/components/ui/input";
import { Label } from "@/components/ui/label";
import {
  Select,
  SelectContent,
  SelectItem,
  SelectTrigger,
  SelectValue,
} from "@/components/ui/select";

import {
  Phone,
  MoveUpRight,
  Star,
  MoveRight,
  CircleCheck,
} from "lucide-vue-next";
</script>

<template>
  <navbar />

  <!-- Header -->
  <div
    class="relative w-full h-screen bg-vector-pattern bg-no-repeat bg-cover bg-center"
  >
    <div class="flex justify-between min-h-screen px-8">
      <div class="flex-1 p-4">
        <h1 class="font-mochi text-txtpurple text-7xl pt-40 ml-10">
          Destinasi Bahagia Untuk Peliharaanmu
        </h1>
        <h3
          class="font-poppins font-bold text-base text-txtgreen py-4 mt-10 ml-10"
        >
          Pusat Kebutuhan Untuk Hewan Peliharaan Anda.<br />
          Terbesar, Terlengkap, dan Terpercaya Di Indonesia
        </h3>
        <div class="flex justify-start items-center space-x-4 ml-10">
          <div>
            <Button
              class="bg-txtpurple rounded-full px-6 py-6 text-base hover:bg-bgpurple"
              >Layanan Kami <MoveUpRight class="ml-2"
            /></Button>
          </div>
          <div>
            <Button
              class="text-txtgreen border-2 border-txtgreen rounded-full px-6 py-6 text-base hover:text-txtgreen"
              variant="outline"
              >Hubungi Kami <Phone class="ml-2"
            /></Button>
          </div>
        </div>
      </div>
      <div class="flex-1 p-4">
        <img
          class="animate-fade-left animate-once animate-delay-200 animate-ease-out animate-alternate"
          src="@/assets/img/cat.png"
          alt="cat"
        />
      </div>
    </div>
  </div>

  <!-- Main -->
  <span id="layanan" />
  <div class="mt-20 mb-32 pt-20 pb-32">
    <h1 class="flex justify-center font-mochi text-4xl text-txtpurple">
      Layanan Kami
    </h1>
    <div class="flex justfify-between item-center px-8 pt-10">
      <div class="px-2">
        <ServiceCard
          icon-src="@/assets/img/iconcat.png"
          title="Dokter Hewan"
          description="Layanan kesehatan hewan peliharaan yang profesional dan terpercaya."
          button-text="Dapatkan Layanan"
          image-src="@/assets/img/cap.png"
        />
      </div>
      <div class="px-2">
        <ServiceCard
          icon-src="@/assets/img/iconcat.png"
          title="Pet Hotel"
          description="Layanan penitipan hewan peliharaan yang nyaman dan aman."
          button-text="Dapatkan Layanan"
          image-src="@/assets/img/cap.png"
        />
      </div>
      <div class="px-2">
        <ServiceCard
          icon-src="@/assets/img/iconcat.png"
          title="Groming"
          description="Layanan perawatan dan kebersihan hewan peliharaan."
          button-text="Dapatkan Layanan"
          image-src="@/assets/img/cap.png"
        />
      </div>
      <div class="px-2">
        <ServiceCard
          icon-src="@/assets/img/iconcat.png"
          title="Pet Shop"
          description="Layanan Kebutuhan hewan peliharaan yang profesional dan terpercaya."
          button-text="Dapatkan Layanan"
          image-src="@/assets/img/cap.png"
        />
      </div>
    </div>
  </div>

  <div class="flex py-10 bg-bggrey place-items-center py-20">
    <div class="flex-1 p-4 ml-32">
      <h1 class="text-3xl font-mochi text-txtpurple my-4">Siapa Kami</h1>
      <p class="font-poppins font-medium">
        Kami adalah sebuah komunitas pecinta hewan yang berkomitmen untuk
        menyediakan fasilitas kesehatan serta layanan untuk hewan peliharaan
        anda
      </p>
      <h1 class="text-3xl font-mochi text-txtpurple my-4">Visi Kami</h1>
      <p class="font-poppins font-medium">
        Kami adalah sebuah komunitas pecinta hewan yang berkomitmen untuk
        menyediakan fasilitas kesehatan serta layanan untuk hewan peliharaan
        anda
      </p>
      <h1 class="text-3xl font-mochi text-txtpurple my-4">Misi Kami</h1>
      <p class="font-poppins font-medium">
        Kami adalah sebuah komunitas pecinta hewan yang berkomitmen untuk
        menyediakan fasilitas kesehatan serta layanan untuk hewan peliharaan
        anda
      </p>
    </div>
    <div class="flex-1 p-4">
      <img src="@/assets/img/cat&dog.png" alt="cat & dog" />
    </div>
  </div>

  <div class="py-10 mx-20">
    <div class="flex justify-center">
      <h1 class="flex justify-center font-mochi text-4xl text-txtpurple">
        Pets Shop
      </h1>
    </div>
    <div class="flex justify-between px-10">
      <div>
        <h2 class="flex justify-center font-mochi text-txtgreen text-lg my-4">
          Produk Baru
        </h2>
        <div>
          <ProductCard
            icon-src="@/assets/img/food.png"
            title="Pedigree Pouch Makanan Basah"
            button-text="Cek Sekarang"
          />
        </div>
        <div>
          <ProductCard
            icon-src="@/assets/img/food.png"
            title="Pedigree Pouch Makanan Basah"
            button-text="Cek Sekarang"
          />
        </div>
        <div>
          <ProductCard
            icon-src="@/assets/img/food.png"
            title="Pedigree Pouch Makanan Basah"
            button-text="Cek Sekarang"
          />
        </div>
      </div>
      <div>
        <h2 class="flex justify-center font-mochi text-txtgreen text-lg my-4">
          Produk Diskon
        </h2>
        <div>
          <ProductCard
            icon-src="@/assets/img/food.png"
            title="Pedigree Pouch Makanan Basah"
            button-text="Cek Sekarang"
          />
        </div>
        <div>
          <ProductCard
            icon-src="@/assets/img/food.png"
            title="Pedigree Pouch Makanan Basah"
            button-text="Cek Sekarang"
          />
        </div>
        <div>
          <ProductCard
            icon-src="@/assets/img/food.png"
            title="Pedigree Pouch Makanan Basah"
            button-text="Cek Sekarang"
          />
        </div>
      </div>
      <div>
        <h2 class="flex justify-center font-mochi text-txtgreen text-lg my-4">
          Produk Unggulan
        </h2>
        <div>
          <ProductCard
            icon-src="@/assets/img/food.png"
            title="Pedigree Pouch Makanan Basah"
            button-text="Cek Sekarang"
          />
        </div>
        <div>
          <ProductCard
            icon-src="@/assets/img/food.png"
            title="Pedigree Pouch Makanan Basah"
            button-text="Cek Sekarang"
          />
        </div>
        <div>
          <ProductCard
            icon-src="@/assets/img/food.png"
            title="Pedigree Pouch Makanan Basah"
            button-text="Cek Sekarang"
          />
        </div>
      </div>
    </div>
  </div>

  <div class="flex justify-around bg-bggrey py-20">
    <div>
      <PriceListCard
        title="Regular Groom"
        price="Rp. 100.000"
        :services="[
          'Dapatkan Layanan',
          'Dapatkan Layanan',
          'Dapatkan Layanan',
          'Dapatkan Layanan',
          'Dapatkan Layanan',
          'Dapatkan Layanan',
        ]"
        buttonText="Cek Sekarang"
      />
    </div>
    <div>
      <PriceListCard
        title="Regular Groom"
        price="Rp. 100.000"
        :services="[
          'Dapatkan Layanan',
          'Dapatkan Layanan',
          'Dapatkan Layanan',
          'Dapatkan Layanan',
          'Dapatkan Layanan',
          'Dapatkan Layanan',
        ]"
        buttonText="Cek Sekarang"
      />
    </div>
    <div>
      <PriceListCard
        title="Regular Groom"
        price="Rp. 100.000"
        :services="[
          'Dapatkan Layanan',
          'Dapatkan Layanan',
          'Dapatkan Layanan',
          'Dapatkan Layanan',
          'Dapatkan Layanan',
          'Dapatkan Layanan',
        ]"
        buttonText="Cek Sekarang"
      />
    </div>
  </div>

  <div class="px-40 py-40 bg-cover bg-no-repeat">
    <div class="w-full h-64 bg-rectangle-pattern bg-no-repeat bg-contain">
      <div class="flex justify-between px-20 pt-20 mx-10">
        <div>
          <h1 class="flex font-mochi text-white text-5xl">
            Peliharaan Anda Aman<br />
            Bersama Kami
          </h1>
        </div>
        <div class="pt-8">
          <Button
            class="font-poppins text-txtgreen border-2 border-txtgreen rounded-full px-6 py-6 text-base hover:text-txtgreen"
            variant="outline"
            >Hubungi Kami
          </Button>
        </div>
      </div>
    </div>
  </div>

  <Footer />
</template>
