<template>
  <Disclosure as="nav" class="fixed top-0 w-full shadow-sm" v-slot="{ open }">
    <div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
      <div class="relative flex h-fit pt-4 items-center justify-between">
        <div class="absolute inset-y-0 left-0 flex items-center sm:hidden">
          <!-- Mobile menu button-->
          <DisclosureButton
            class="relative inline-flex items-center justify-center rounded-md p-2 text-slate-400 hover:bg-slate-700 hover:text-white focus:outline-none focus:ring-2 focus:ring-inset focus:ring-white"
          >
            <span class="absolute -inset-0.5" />
            <span class="sr-only">Open main menu</span>
          </DisclosureButton>
        </div>
        <div class="flex flex-1 items-center justify-center sm:items-stretch sm:justify-start">
          <div class="hidden sm:ml-6 sm:block">
            <div class="flex space-x-4">
              <a
                v-for="item in navigation"
                :key="item.name"
                :href="item.href"
                :class="[
                  'text-lg border-b-2 hover:border-slate-200 px-3 pt-2 pb-4 font-medium',
                  item.current
                    ? 'text-sky-600 hover:text-sky-700 border-sky-500 hover:border-sky-600'
                    : 'text-slate-400 hover:text-slate-500 border-transparent hover:border-slate-300'
                ]"
                :aria-current="item.current ? 'page' : undefined"
              >
                <h3>{{ item.name }}</h3>
              </a>
            </div>
          </div>
        </div>
        <div class="flex items-center pr-2">
          <button type="button" class="p-1 rounded-md">🇫🇷</button>
          <button type="button" class="p-1 rounded-md">🇬🇧</button>
        </div>
      </div>
    </div>

    <DisclosurePanel class="sm:hidden">
      <div class="space-y-1 px-2 pb-3 pt-2">
        <DisclosureButton
          v-for="item in navigation"
          :key="item.name"
          as="a"
          :href="item.href"
          :class="[
            item.current
              ? 'bg-slate-900 text-white'
              : 'text-slate-300 hover:bg-slate-700 hover:text-white',
            'block rounded-md px-3 py-2 text-base font-medium'
          ]"
          :aria-current="item.current ? 'page' : undefined"
          >{{ item.name }}</DisclosureButton
        >
      </div>
    </DisclosurePanel>
  </Disclosure>
</template>

<script setup>
import {
  Disclosure,
  DisclosureButton,
  DisclosurePanel,
  Menu,
  MenuButton,
  MenuItem,
  MenuItems
} from '@headlessui/vue'

const navigation = [
  { name: 'Présentation', href: '#', current: true },
  { name: 'Portfolio', href: '#', current: false }
]
</script>
