---
layout: carouselLayout
---

<script>
	import { Card, Breadcrumb } from '$lib/index';
	let divClass = 'max-w-xs bg-white rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700';
	  let crumbs = [
    {
      label:'Home',
      href:'/'
    },
    {
      label:'Carousels',
      href:'/carousels/'
    },
  ]
</script>

<Breadcrumb {crumbs}/>

<h1 class="text-3xl w-full dark:text-white py-8">Carousel Components</h1>

<div class="p-4">
	<Card {divClass} img="/images/carousel.webp" btnColor="blue" header="CAROUSEL" link="/carousels/default" btnLabel="Read more" />
</div>
<div class="p-4">
	<Card {divClass} img="/images/carousel.webp" btnColor="blue" header="CAROUSEL TRANSITION" link="/carousels/transition" btnLabel="Read more" />
</div>
