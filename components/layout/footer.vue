<script lang="ts">
import { Separator } from "../ui/separator";

import {
  NavigationMenu,
  NavigationMenuItem,
  NavigationMenuLink,
  NavigationMenuList,
  navigationMenuTriggerStyle,
} from "@/components/ui/navigation-menu";

export default {
  name: "Footer",
  methods: {
    scrollToTop() {
      window.scrollTo({ top: 0, behavior: "smooth" });
    },
  },
};
</script>

<template>
  <div
    class="bg-footer-pattern bg-no-repeat bg-cover w-full h-full text-white font-poppins"
  >
  <div class="mx-24">
    <div class="flex justify-between mx-20 pt-10 text-white">
      <div>
        <NuxtLink to="/" @click.native="scrollToTop">
          <img src="~/assets/img/logowhite.png" alt="logo" />
        </NuxtLink>
        <p class="ml-10">
          Pusat Kebutuhan Untuk<br />
          Hewan Peliharaan Anda.<br />
          Terbesar, Terlengkap ,<br />
          dan Terpercaya Di Indonesia.
        </p>
      </div>
      <div>
        <h2 class="font-bold">Fitur Kami</h2>
        <NavigationMenu>
          <NavigationMenuList>
            <NavigationMenuItem>
              <div class="py-4">
                <div>
                  <NavigationMenuLink class="bg-inherit hover:text-txtgreen">
                    <NuxtLink to="/" @click.native="scrollToTop"
                      >Home</NuxtLink
                    >
                  </NavigationMenuLink>
                </div>
                <div>
                  <NavigationMenuLink class="bg-inherit hover:text-txtgreen">
                    <NuxtLink to="#layanan">Layanan</NuxtLink>
                  </NavigationMenuLink>
                </div>
                <div>
                  <NavigationMenuLink class="bg-inherit hover:text-txtgreen">
                    <NuxtLink to="/">PetShop</NuxtLink>
                  </NavigationMenuLink>
                </div>
                <div>
                  <NavigationMenuLink class="bg-inherit hover:text-txtgreen">
                    <NuxtLink to="/">Dokter Hewan</NuxtLink>
                  </NavigationMenuLink>
                </div>
                <div>
                  <NavigationMenuLink class="bg-inherit hover:text-txtgreen">
                    <NuxtLink to="/">Tentang Kami</NuxtLink>
                  </NavigationMenuLink>
                </div>
              </div>
            </NavigationMenuItem>
          </NavigationMenuList>
        </NavigationMenu>
      </div>
      <div>
        <h2 class="font-bold">Hubungi Kami</h2>
        <p class="pt-4">
          Jalan Bojongsoang No. 17 <br />
          <b>Kontak:</b> 08123456789 <br />
          <b>Email:</b><br />
          petcare@cat.mail <br />
        </p>
      </div>
      <div>
        <h2 class="font-bold">Layanan</h2>
        <NavigationMenu>
          <NavigationMenuList>
            <NavigationMenuItem>
              <div class="py-4">
                <div>
                  <NavigationMenuLink class="bg-inherit hover:text-txtgreen">
                    <NuxtLink to="/" @click.native="scrollToTop"
                      >Pet Shop</NuxtLink
                    >
                  </NavigationMenuLink>
                </div>
                <div>
                  <NavigationMenuLink class="bg-inherit hover:text-txtgreen">
                    <NuxtLink to="#layanan">Groming</NuxtLink>
                  </NavigationMenuLink>
                </div>
                <div>
                  <NavigationMenuLink class="bg-inherit hover:text-txtgreen">
                    <NuxtLink to="/">Dokter Hewan</NuxtLink>
                  </NavigationMenuLink>
                </div>
              </div>
            </NavigationMenuItem>
          </NavigationMenuList>
        </NavigationMenu>
      </div>
    </div>
  </div>
    
    <div class="my-5 px-20">
      <Separator />
    </div>

    <h1 class="flex justify-center">
      © Copyright &nbsp; <b>PetCare.</b> &nbsp; All Rights Reserved
    </h1>
  </div>
</template>
