<script setup lang="ts">
import { Button, Input, FormItem } from '@/components/m'
import Img from '@/assets/images/auth.png'
</script>
<template>
  <main class="flex justify-center bg-foreground-primary text-white min-h-screen">
    <section class="w-1/3 py-10 px-10 h-full">
      <div class="mb-16">
        <div class="text-3xl font-semibold">Welcome Back 👋</div>
        <div class="text-white">We are happy to have you back</div>
      </div>
      <form class="space-y-3">
        <FormItem id="fullName" label="FullName" class="w-full">
          <Input id="fullName" color="default" placeholder="Enter your Name" class="w-full" />
        </FormItem>
        <FormItem id="email" label="email" class="w-full">
          <Input
            id="email"
            type="email"
            color="default"
            placeholder="Enter your Email"
            class="w-full"
          />
        </FormItem>
        <FormItem id="password" label="password" class="w-full">
          <Input
            id="password"
            type="password"
            color="default"
            placeholder="Enter your password"
            class="w-full"
          />
        </FormItem>
        <div>
          <Button class="block w-full mt-5" color="primary">Register</Button>
        </div>
      </form>
    </section>
    <section class="flex-1 h-full p-5">
      <div class="rounded-lg overflow-hidden">
        <img class="w-full object-cover" :src="Img" alt="" />
      </div>
    </section>
  </main>
</template>

<style scoped></style>
