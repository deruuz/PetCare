<script setup lang="ts">
import navbar from "@/components/layout/navbar.vue";
import Footer from "@/components/layout/footer.vue";

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

import { Phone , MoveUpRight } from "lucide-vue-next";

</script>

<template>
  <navbar />
  <div
    class="relative w-full h-screen bg-vector-pattern bg-no-repeat bg-cover bg-center"
  >
    <div class="flex justify-between min-h-screen px-8">
      <div class="flex-1 p-4">
        <h1 class="font-mochi text-5xl pt-60">
          Destinasi Kebahagiaan Untuk Peliharaanmu
        </h1>
        <h3 class="font-mochi text-xs text-green-400 py-4">
          Pusat Kebutuhan Untuk Hewan Peliharaan Anda.<br >
          Terbesar, Terlengkap, dan Terpercaya Di Indonesia
        </h3>
        <div class="flex justify-start items-center space-x-4">
          <div>
            <Button>Layanan Kami <MoveUpRight /></Button>
          </div>
          <div>
            <Button>Hubungi Kami <Phone /></Button>
          </div>
        </div>
      </div>
      <div class="flex-1 p-4">
        <img src="@/assets/img/cat.png" alt="cat" >
      </div>
    </div>
  </div>
  <div class="pt-10 pb-60">
    <h1 class="flex justify-center font-mochi text-3xl">Layanan Kami</h1>
    <div class="flex justfify-between item-center px-8 pt-10">
      <div class="px-2">
        <Card class="w-[350px]">
          <CardHeader>
            <CardTitle>Create project</CardTitle>
            <CardDescription
              >Deploy your new project in one-click.</CardDescription
            >
          </CardHeader>
          <CardContent>
            <form>
              <div class="grid items-center w-full gap-4">
                <div class="flex flex-col space-y-1.5">
                  <Label for="name">Name</Label>
                  <Input id="name" placeholder="Name of your project" />
                </div>
                <div class="flex flex-col space-y-1.5">
                  <Label for="framework">Framework</Label>
                  <Select>
                    <SelectTrigger id="framework">
                      <SelectValue placeholder="Select" />
                    </SelectTrigger>
                    <SelectContent position="popper">
                      <SelectItem value="nuxt"> Nuxt </SelectItem>
                      <SelectItem value="next"> Next.js </SelectItem>
                      <SelectItem value="sveltekit"> SvelteKit </SelectItem>
                      <SelectItem value="astro"> Astro </SelectItem>
                    </SelectContent>
                  </Select>
                </div>
              </div>
            </form>
          </CardContent>
          <CardFooter class="flex justify-between px-6 pb-6">
            <Button variant="outline"> Cancel </Button>
            <Button>Deploy</Button>
          </CardFooter>
        </Card>
      </div>
      <div class="px-2">
        <Card class="w-[350px]">
          <CardHeader>
            <CardTitle>Create project</CardTitle>
            <CardDescription
              >Deploy your new project in one-click.</CardDescription
            >
          </CardHeader>
          <CardContent>
            <form>
              <div class="grid items-center w-full gap-4">
                <div class="flex flex-col space-y-1.5">
                  <Label for="name">Name</Label>
                  <Input id="name" placeholder="Name of your project" />
                </div>
                <div class="flex flex-col space-y-1.5">
                  <Label for="framework">Framework</Label>
                  <Select>
                    <SelectTrigger id="framework">
                      <SelectValue placeholder="Select" />
                    </SelectTrigger>
                    <SelectContent position="popper">
                      <SelectItem value="nuxt"> Nuxt </SelectItem>
                      <SelectItem value="next"> Next.js </SelectItem>
                      <SelectItem value="sveltekit"> SvelteKit </SelectItem>
                      <SelectItem value="astro"> Astro </SelectItem>
                    </SelectContent>
                  </Select>
                </div>
              </div>
            </form>
          </CardContent>
          <CardFooter class="flex justify-between px-6 pb-6">
            <Button variant="outline"> Cancel </Button>
            <Button>Deploy</Button>
          </CardFooter>
        </Card>
      </div>
      <div class="px-2">
        <Card class="w-[350px]">
          <CardHeader>
            <CardTitle>Create project</CardTitle>
            <CardDescription
              >Deploy your new project in one-click.</CardDescription
            >
          </CardHeader>
          <CardContent>
            <form>
              <div class="grid items-center w-full gap-4">
                <div class="flex flex-col space-y-1.5">
                  <Label for="name">Name</Label>
                  <Input id="name" placeholder="Name of your project" />
                </div>
                <div class="flex flex-col space-y-1.5">
                  <Label for="framework">Framework</Label>
                  <Select>
                    <SelectTrigger id="framework">
                      <SelectValue placeholder="Select" />
                    </SelectTrigger>
                    <SelectContent position="popper">
                      <SelectItem value="nuxt"> Nuxt </SelectItem>
                      <SelectItem value="next"> Next.js </SelectItem>
                      <SelectItem value="sveltekit"> SvelteKit </SelectItem>
                      <SelectItem value="astro"> Astro </SelectItem>
                    </SelectContent>
                  </Select>
                </div>
              </div>
            </form>
          </CardContent>
          <CardFooter class="flex justify-between px-6 pb-6">
            <Button variant="outline"> Cancel </Button>
            <Button>Deploy</Button>
          </CardFooter>
        </Card>
      </div>
      <div class="px-2">
        <Card class="w-[350px]">
          <CardHeader>
            <CardTitle>Create project</CardTitle>
            <CardDescription
              >Deploy your new project in one-click.</CardDescription
            >
          </CardHeader>
          <CardContent>
            <form>
              <div class="grid items-center w-full gap-4">
                <div class="flex flex-col space-y-1.5">
                  <Label for="name">Name</Label>
                  <Input id="name" placeholder="Name of your project" />
                </div>
                <div class="flex flex-col space-y-1.5">
                  <Label for="framework">Framework</Label>
                  <Select>
                    <SelectTrigger id="framework">
                      <SelectValue placeholder="Select" />
                    </SelectTrigger>
                    <SelectContent position="popper">
                      <SelectItem value="nuxt"> Nuxt </SelectItem>
                      <SelectItem value="next"> Next.js </SelectItem>
                      <SelectItem value="sveltekit"> SvelteKit </SelectItem>
                      <SelectItem value="astro"> Astro </SelectItem>
                    </SelectContent>
                  </Select>
                </div>
              </div>
            </form>
          </CardContent>
          <CardFooter class="flex justify-between px-6 pb-6">
            <Button variant="outline"> Cancel </Button>
            <Button>Deploy</Button>
          </CardFooter>
        </Card>
      </div>
    </div>
  </div>

  <div class="flex pt-60 pb-60">
    <div class="flex-1 p-4 ">
      <h1 class="text-lg font-mochi">Siapa Kami</h1>
      <p>
        Kami adalah sebuah komunitas pecinta hewan yang berkomitmen untuk menyediakan fasilitas kesehatan serta layanan untuk hewan peliharaan anda
      </p>
      <h1 class="font-mochi"> Visi Kami</h1>
      <p>Kami adalah sebuah komunitas pecinta hewan yang berkomitmen untuk menyediakan fasilitas kesehatan serta layanan untuk hewan peliharaan anda</p>
      <h1 class="font-mochi"> Misi Kami</h1>
      <p>
        Kami adalah sebuah komunitas pecinta hewan yang berkomitmen untuk menyediakan fasilitas kesehatan serta layanan untuk hewan peliharaan anda
      </p>
    </div>
    <div class="flex-1 p-4">
      <img src="@/assets/img/cat&dog.png" alt="cat & dog" >
    </div>
  </div>
  <Footer />
</template>
