<script setup lang="ts">
import {
  NavigationMenu,
  NavigationMenuItem,
  NavigationMenuLink,
  NavigationMenuList,
  navigationMenuTriggerStyle,
} from "@/components/ui/navigation-menu";
</script>

<template>
  <div class="flex justify-between items-center bg-bgpurple py-4">
    <div class="pl-8 flex justify-start">
      <img src="@/assets/img/logo.png" alt="logo" >
    </div>
    <NavigationMenu>
      <NavigationMenuList>
        <NavigationMenuItem>
            <div class="flex justify-between items-center">
                <div class="px-2">
            <NavigationMenuLink :class="navigationMenuTriggerStyle()">
              <NuxtLink to="/">Home</NuxtLink>
            </NavigationMenuLink>
          </div>
          <div class="px-2">
            <NavigationMenuLink :class="navigationMenuTriggerStyle()">
              <NuxtLink to="/">Layanan</NuxtLink>
            </NavigationMenuLink>
          </div>
          <div class="px-2">
            <NavigationMenuLink :class="navigationMenuTriggerStyle()">
              <NuxtLink to="/">Dokter Hewan</NuxtLink>
            </NavigationMenuLink>
          </div>
          <div class="px-2">
            <NavigationMenuLink :class="navigationMenuTriggerStyle()">
              <NuxtLink to="/">Tentang Kami</NuxtLink>
            </NavigationMenuLink>
          </div>
            </div>
          
        </NavigationMenuItem>
      </NavigationMenuList>
    </NavigationMenu>
  </div>
</template>
