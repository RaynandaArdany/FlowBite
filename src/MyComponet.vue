<script setup>
import { Navbar, NavbarLogo, NavbarCollapse, NavbarLink } from 'flowbite-vue'
import { ref } from 'vue'
import { Tabs, Tab } from 'flowbite-vue'
import { TheCard } from 'flowbite-vue'
const activeTab = ref('first')
import { Carousel } from 'flowbite-vue'
import { Timeline, TimelineItem, TimelinePoint, TimelineTime, TimelineContent, TimelineTitle } from 'flowbite-vue'
import { Footer } from 'flowbite-vue'
import { Avatar } from 'flowbite-vue'
const pictures = [
  {
    'src': 'https://flowbite.s3.amazonaws.com/docs/gallery/featured/image.jpg',
    'alt': 'Picture 1',
  },
  {
    'src': 'https://flowbite.s3.amazonaws.com/docs/gallery/square/image-1.jpg',
    'alt': 'Picture 2',
  },
  {
    'src': 'https://flowbite.s3.amazonaws.com/docs/gallery/square/image-2.jpg',
    'alt': 'Picture 3',
  },
  {
    'src': 'https://flowbite.s3.amazonaws.com/docs/gallery/square/image-3.jpg',
    'alt': 'Picture 4',
  },
  {
    'src': 'https://flowbite.s3.amazonaws.com/docs/gallery/square/image-5.jpg',
    'alt': 'Picture 5',
  },
]
</script>


<template>
    <Navbar>
      <template #logo>
        <NavbarLogo link="https://www.google.com/" alt="Flowbite logo" image-url="https://flowbite.com/docs/images/logo.svg">
          New News
        </NavbarLogo>
      </template>
      <template #default="{isShowMenu}">
        <NavbarCollapse :isShowMenu="isShowMenu">
          <NavbarLink is-active>Beranda</NavbarLink>
          <NavbarLink>Tentang</NavbarLink>
          <NavbarLink>Kontak</NavbarLink>
        </NavbarCollapse>
      </template>
      <template #menu-icon>
        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6V4m0 2a2 2 0 100 4m0-4a2 2 0 110 4m-6 8a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4m6 6v10m6-2a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4"></path></svg>
      </template>
    </Navbar>

    <Carousel :pictures="pictures"></Carousel>

  <tabs variant="underline" v-model="activeTab" class="p-5"> <!-- class appends to content DIV for all tabs -->
    <tab name="Temukan" title="Temukan">
<div class="flex items-center">

    <the-card class="mr-20" variant="image" img-src="https://flowbite.com/docs/images/blog/image-1.jpg" img-alt="Desk">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy technology acquisitions 2021</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
      Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.
    </p>
  </the-card>

  <the-card class="mr-20" variant="image" img-src="https://flowbite.com/docs/images/blog/image-1.jpg" img-alt="Desk">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy technology acquisitions 2021</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
      Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.
    </p>
  </the-card>

  <the-card class="mr-2" variant="image" img-src="https://flowbite.com/docs/images/blog/image-1.jpg" img-alt="Desk">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy technology acquisitions 2021</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
      Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.
    </p>
  </the-card>

</div>
<br>
<div class="flex items-center">

<the-card class="mr-20" variant="image" img-src="https://flowbite.com/docs/images/blog/image-1.jpg" img-alt="Desk">
<h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy technology acquisitions 2021</h5>
<p class="font-normal text-gray-700 dark:text-gray-400">
  Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.
</p>
</the-card>

<the-card class="mr-20" variant="image" img-src="https://flowbite.com/docs/images/blog/image-1.jpg" img-alt="Desk">
<h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy technology acquisitions 2021</h5>
<p class="font-normal text-gray-700 dark:text-gray-400">
  Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.
</p>
</the-card>

<the-card class="mr-2" variant="image" img-src="https://flowbite.com/docs/images/blog/image-1.jpg" img-alt="Desk">
<h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy technology acquisitions 2021</h5>
<p class="font-normal text-gray-700 dark:text-gray-400">
  Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.
</p>
</the-card>

</div>
 
    </tab>
    <tab name="Berita" title="Berita">
        <div class="flex">
        <the-card class="mr-5" href="#" variant="horizontal" img-src="https://flowbite.com/docs/images/blog/image-4.jpg" img-alt="Desk">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy technology acquisitions 2021</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
      Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.
    </p>
  </the-card>

  <the-card class="mr-5" href="#" variant="horizontal" img-src="https://flowbite.com/docs/images/blog/image-4.jpg" img-alt="Desk">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy technology acquisitions 2021</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
      Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.
    </p>
  </the-card>

  <the-card href="#">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy technology acquisitions 2021</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
      Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.
    </p>
  </the-card>
</div>
<br>
<div class="flex">
        <the-card class="mr-5" href="#" variant="horizontal" img-src="https://flowbite.com/docs/images/blog/image-4.jpg" img-alt="Desk">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy technology acquisitions 2021</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
      Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.
    </p>
  </the-card>

  <the-card class="mr-5" href="#" variant="horizontal" img-src="https://flowbite.com/docs/images/blog/image-4.jpg" img-alt="Desk">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy technology acquisitions 2021</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
      Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.
    </p>
  </the-card>

  <the-card href="#">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy technology acquisitions 2021</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
      Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.
    </p>
  </the-card>
</div>
    </tab>
    <tab name="Game Visual" title="Game Visual">
        <div class="flex">
        <the-card class="mr-5" href="#" variant="horizontal" img-src="https://flowbite.com/docs/images/blog/image-4.jpg" img-alt="Desk">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy technology acquisitions 2021</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
      Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.
    </p>
  </the-card>

  <the-card class="mr-5" href="#" variant="horizontal" img-src="https://flowbite.com/docs/images/blog/image-4.jpg" img-alt="Desk">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy technology acquisitions 2021</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
      Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.
    </p>
  </the-card>

  <the-card href="#">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy technology acquisitions 2021</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
      Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.
    </p>
  </the-card>
</div>
    </tab>
    <tab name="Akan Datang" title="Akan Datang" :disabled="true">
      Lorem...
    </tab>
  </tabs>

  <Timeline horizontal>
    <timeline-item>
      <timeline-point>
        <svg aria-hidden="true" class="w-3 h-3 text-blue-600 dark:text-blue-400" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z" clip-rule="evenodd"></path></svg>
      </timeline-point>
      <timeline-content>
        <timeline-time>
          February 2022
        </timeline-time>
        <timeline-title>
          Application UI code in Tailwind CSS
        </timeline-title>
        <timeline-body>
          Get access to over 20+ pages including a dashboard layout, charts, kanban board, calendar, and pre-order E-commerce & Marketing pages.
        </timeline-body>
      </timeline-content>
    </timeline-item>
    <timeline-item>
      <timeline-point>
        <svg aria-hidden="true" class="w-3 h-3 text-blue-600 dark:text-blue-400" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z" clip-rule="evenodd"></path></svg>
      </timeline-point>
      <timeline-content>
        <timeline-time>
          February 2022
        </timeline-time>
        <timeline-title>
          Application UI code in Tailwind CSS
        </timeline-title>
        <timeline-body>
          Get access to over 20+ pages including a dashboard layout, charts, kanban board, calendar, and pre-order E-commerce & Marketing pages.
        </timeline-body>
      </timeline-content>
    </timeline-item>
    <timeline-item>
      <timeline-point>
        <svg aria-hidden="true" class="w-3 h-3 text-blue-600 dark:text-blue-400" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z" clip-rule="evenodd"></path></svg>
      </timeline-point>
      <timeline-content>
        <timeline-time>
          February 2022
        </timeline-time>
        <timeline-title>
          Application UI code in Tailwind CSS
        </timeline-title>
        <timeline-body>
          Get access to over 20+ pages including a dashboard layout, charts, kanban board, calendar, and pre-order E-commerce & Marketing pages.
        </timeline-body>
      </timeline-content>
    </timeline-item>
  </Timeline>

  <Footer></Footer>
</template>
