---
layout: badgeLayout
---

<script>
  import Htwo from '../utils/Htwo.svelte'
  import ExampleDiv from '../utils/ExampleDiv.svelte'
  import TableProp from '../utils/TableProp.svelte'
  import TableDefaultRow from '../utils/TableDefaultRow.svelte'
  import {BadgeLink, Breadcrumb } from "$lib/index"
  import componentProps from '../props/BadgeLink.json'
  // Props table
  let items = componentProps.props
	let propHeader = ['Name', 'Type', 'Default']
	
	let divClass='w-full relative overflow-x-auto shadow-md sm:rounded-lg py-4'
let theadClass ='text-xs text-gray-700 uppercase bg-gray-50 dark:bg-gray-700 dark:text-white'

  let link="/"
    let crumbs = [
    {
      label:'Home',
      href:'/'
    },
    {
      label:'Badges',
      href:'/badges/'
    },
    {
      label:'Link badge',
      href:'/badges/badge-link'
    }
  ]
</script>

<Breadcrumb {crumbs}/>

<h1 class="text-3xl w-full dark:text-white py-8">Badges with Link</h1>

```html
<script>
  import {BadgeLink} from 'flowbite-svelte'
  let link="/"
</script>
```

<Htwo label="Size xs" />

<ExampleDiv>
<BadgeLink name="Default" {link}/>
<BadgeLink name="Gray" color="gray" {link}/>
<BadgeLink name="Red" color="red" {link}/>
<BadgeLink name="Green" color="green" {link}/>
<BadgeLink name="Yellow" color="yellow" {link}/>
<BadgeLink name="Indigo" color="indigo" {link}/>
<BadgeLink name="Purple" color="purple" {link}/>
<BadgeLink name="Pink" color="pink" {link}/>
</ExampleDiv>

```html
<BadgeLink name="Default" {link}/>
<BadgeLink name="Gray" color="gray" {link}/>
<BadgeLink name="Red" color="red" {link}/>
<BadgeLink name="Green" color="green" {link}/>
<BadgeLink name="Yellow" color="yellow" {link}/>
<BadgeLink name="Indigo" color="indigo" {link}/>
<BadgeLink name="Purple" color="purple" {link}/>
<BadgeLink name="Pink" color="pink" {link}/>
```

<Htwo label="Size sm" />

<ExampleDiv>
<BadgeLink name="Default" textSize="text-sm" {link}/>
<BadgeLink name="Gray" color="gray" textSize="text-sm" {link}/>
<BadgeLink name="Red" color="red" textSize="text-sm" {link}/>
<BadgeLink name="Green" color="green" textSize="text-sm" {link}/>
<BadgeLink name="Yellow" color="yellow" textSize="text-sm" {link}/>
<BadgeLink name="Indigo" color="indigo" textSize="text-sm" {link}/>
<BadgeLink name="Purple" color="purple" textSize="text-sm" {link}/>
<BadgeLink name="Pink" color="pink" textSize="text-sm" {link}/>
</ExampleDiv>

```html
<BadgeLink name="Default" textSize="text-sm" {link}/>
<BadgeLink name="Gray" color="gray" textSize="text-sm" {link}/>
<BadgeLink name="Red" color="red" textSize="text-sm" {link}/>
<BadgeLink name="Green" color="green" textSize="text-sm" {link}/>
<BadgeLink name="Yellow" color="yellow" textSize="text-sm" {link}/>
<BadgeLink name="Indigo" color="indigo" textSize="text-sm" {link}/>
<BadgeLink name="Purple" color="purple" textSize="text-sm" {link}/>
<BadgeLink name="Pink" color="pink" textSize="text-sm" {link}/>
```

<Htwo label="Size base" />

<ExampleDiv>
<BadgeLink name="Default" textSize="text-base" {link}/>
<BadgeLink name="Gray" color="gray" textSize="text-base" {link}/>
<BadgeLink name="Red" color="red" textSize="text-base" {link}/>
<BadgeLink name="Green" color="green" textSize="text-base" {link}/>
<BadgeLink name="Yellow" color="yellow" textSize="text-base" {link}/>
<BadgeLink name="Indigo" color="indigo" textSize="text-base" {link}/>
<BadgeLink name="Purple" color="purple" textSize="text-base" {link}/>
<BadgeLink name="Pink" color="pink" textSize="text-base" {link}/>
</ExampleDiv>

```html
<BadgeLink name="Default" textSize="text-base" {link}/>
<BadgeLink name="Gray" color="gray" textSize="text-base" {link}/>
<BadgeLink name="Red" color="red" textSize="text-base" {link}/>
<BadgeLink name="Green" color="green" textSize="text-base" {link}/>
<BadgeLink name="Yellow" color="yellow" textSize="text-base" {link}/>
<BadgeLink name="Indigo" color="indigo" textSize="text-base" {link}/>
<BadgeLink name="Purple" color="purple" textSize="text-base" {link}/>
<BadgeLink name="Pink" color="pink" textSize="text-base" {link}/>
```

<Htwo label="Props" />

<p>The component has the following props, type, and default values. See <a href="/pages/types">types 
 page</a> for type information.</p>

<TableProp header={propHeader} {divClass} {theadClass}>
  <TableDefaultRow {items} rowState='hover' />
</TableProp>