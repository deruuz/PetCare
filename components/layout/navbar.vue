<script setup lang="ts">
import {
  NavigationMenu,
  NavigationMenuItem,
  NavigationMenuLink,
  NavigationMenuList,
  navigationMenuTriggerStyle,
} from "@/components/ui/navigation-menu";

function scrollToTop() {
  window.scrollTo({ top: 0, behavior: 'smooth' });
}
</script>

<template>
  <div class="fixed top-0 left-0 w-full z-50 flex justify-between items-center bg-bgpurple py-4 ">
    <div class="pl-8 flex justify-start">
      <NuxtLink to="/" @click.native="scrollToTop">
      <img src="@/assets/img/Logo.png" alt="logo">
    </NuxtLink>
    </div>
    <NavigationMenu>
      <NavigationMenuList>
        <NavigationMenuItem>
            <div class="flex justify-between items-center font-mochi text-txtpurple">
                <div class="px-2">
            <NavigationMenuLink class="bg-inherit hover:text-txtpurple" :class="navigationMenuTriggerStyle()">
              <NuxtLink to="/" @click.native="scrollToTop">Home</NuxtLink>
            </NavigationMenuLink>
          </div>
          <div class="px-2">
            <NavigationMenuLink class="bg-inherit hover:text-txtpurple" :class="navigationMenuTriggerStyle()">
              <NuxtLink to="#layanan">Layanan</NuxtLink>
            </NavigationMenuLink>
          </div>
          <div class="px-2">
            <NavigationMenuLink class="bg-inherit hover:text-txtpurple" :class="navigationMenuTriggerStyle()">
              <NuxtLink to="/">Dokter Hewan</NuxtLink>
            </NavigationMenuLink>
          </div>
          <div class="px-2">
            <NavigationMenuLink class="bg-inherit hover:text-txtpurple" :class="navigationMenuTriggerStyle()">
              <NuxtLink to="/">Tentang Kami</NuxtLink>
            </NavigationMenuLink>
          </div>
            </div>
          
        </NavigationMenuItem>
      </NavigationMenuList>
    </NavigationMenu>
  </div>
</template>
