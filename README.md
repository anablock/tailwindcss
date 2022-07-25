# README

* `class="md:flex"`

## Classes
* `bg-...` - background
* `p-0` - padding
* `pl-8` - padding left
* `pt-8` - padding top
* `px-8` - padding horizontal (x - axis)
* `py-8` - padding vertical (y - axis)
* `h-10` - height
* `rounded-lg` - rounded corners
* `shadow-xl` - 
* `mt-6` - margin top
* `text-...` - use to change font size and text color
* `font-thin` - font weight
* `text-gray-900` - common for designers to use this gray instead of black to make it easier on users' eyes.
* `space-y-2` - vertical spacing utility.  Use it to replace multiple common attributes to elements.
* `inline-block` - use on buttons 
* `uppercase` - When using uppercase, increase letter spacing by using `tracking-wider` and `font-semibold`
* `relative` - 
* `flex` - Utilities for controlling how flex items both grow and shrink.
* `items` - Utilities for controlling how flex and grid items are positioned along a container's cross axis.
* Use justify-between to justify items along the container’s main axis such that there is an equal amount of space between each item

### Image Cropping
* `object-center`

### Responsiveness
* `max-w-md` - max width container
* `mx-auto` - center the container
Tailwind comes with 5 css breakpoints:
*   {
        "sm": "640px",
        "md": "768px",
        "lg": "1024px",
        "xl": "1280px",
        "2xl": "1536px
    }
* targeting a small breakpoint in an element tag:
    * `sm:max-w-xl`
### Nesting
```html
    <!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <link rel="stylesheet" href="/css/tailwind.css" />
  </head>
  <body class="bg-gray-300">
    <div class="grid bg-gray-100 lg:grid-cols-2 2xl:grid-cols-5">
      <div
        class="max-w-md px-8 py-12 mx-auto sm:max-w-xl lg:px-12 lg:py-24 lg:max-w-full xl:mr-0 2xl:col-span-2"
      >
        <div class="xl:max-w-xl">
          <img class="h-10" src="/img/logo.svg" alt="Workcation" />
          <img
            class="object-center mt-6 rounded-lg shadow-xl sm:mt-8 sm:h-64 sm:w-full sm:object-cover lg:hidden"
            src="/img/beach-work.jpg"
            alt="Woman workcationing on the beach"
          />
          <h1
            class="mt-6 text-2xl font-bold text-gray-900 sm:mt-8 sm:text-4xl lg:text-3xl xl:text-4xl"
          >
            You can work from anywhere.
            <br class="hidden lg:inline" />
            <span class="text-indigo-500">Take advantage of it.</span>
          </h1>
          <p class="mt-2 text-gray-600 sm:mt-4 sm:text-xl">
            Workcation helps you find work-friendly rentals in beautiful locations so you can enjoy
            some nice weather even when you're not on vacation.
          </p>
          <div class="mt-4 sm:mt-6">
            <a
              class="inline-block px-5 py-3 rounded-lg transform transition bg-indigo-500 hover:bg-indigo-400 hover:-translate-y-0.5 focus:ring-indigo-500 focus:ring-opacity-50 focus:outline-none focus:ring focus:ring-offset-2 active:bg-indigo-600 uppercase tracking-wider font-semibold text-sm text-white shadow-lg sm:text-base"
              href="#"
            >
              Book your escape
            </a>
          </div>
        </div>
      </div>
      <div class="relative hidden lg:block 2xl:col-span-3">
        <img
          class="absolute inset-0 object-cover object-center w-full h-full"
          src="/img/beach-work.jpg"
          alt="Woman workcationing on the beach"
        />
      </div>
    </div>
  </body>
</html>
```
### Example
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <link rel="stylesheet" href="/css/tailwind.css" />
  </head>
  <body class="bg-gray-300">
    <div class="grid bg-gray-100 lg:grid-cols-2 2xl:grid-cols-5">
      <div
        class="max-w-md px-8 py-12 mx-auto sm:max-w-xl lg:px-12 lg:py-24 lg:max-w-full xl:mr-0 2xl:col-span-2"
      >
        <div class="xl:max-w-xl">
          <img class="h-10" src="/img/logo.svg" alt="Workcation" />
          <img
            class="object-center mt-6 rounded-lg shadow-xl sm:mt-8 sm:h-64 sm:w-full sm:object-cover lg:hidden"
            src="/img/beach-work.jpg"
            alt="Woman workcationing on the beach"
          />
          <h1
            class="mt-6 text-2xl font-bold text-gray-900 sm:mt-8 sm:text-4xl lg:text-3xl xl:text-4xl"
          >
            You can work from anywhere.
            <br class="hidden lg:inline" />
            <span class="text-indigo-500">Take advantage of it.</span>
          </h1>
          <p class="mt-2 text-gray-600 sm:mt-4 sm:text-xl">
            Workcation helps you find work-friendly rentals in beautiful locations so you can enjoy
            some nice weather even when you're not on vacation.
          </p>
          <div class="mt-4 space-x-1 sm:mt-6">
            <a
              class="btn btn-primary shadow-lg transform transition hover:-translate-y-0.5"
              href="#"
              >Book your escape</a
            >
            <a class="btn btn-secondary" href="#">Learn more</a>
          </div>
        </div>
      </div>
      <div class="relative hidden lg:block 2xl:col-span-3">
        <img
          class="absolute inset-0 object-cover object-center w-full h-full"
          src="/img/beach-work.jpg"
          alt="Woman workcationing on the beach"
        />
      </div>
    </div>
  </body>
</html>
```


## Commands
* `npx tailwindcss -o build.css --minify`
* `npx tailwindcss-cli build tailwind.css -o build/tailwind.css`
* `npm init -y`
* `npm install -D tailwindcss postcss autoprefixer vite`
* `npx tailwindcss init -p`
* `npm run dev`
* `npx tailwindcss init tailwind-full.config.js --full`

##

```html
<div class="flex items-center max-w-sm p-6 mx-auto space-x-4 bg-white shadow-lg rounded-xl">
  <div class="shrink-0">
    <img class="w-12 h-12" src="/img/logo.svg" alt="ChitChat Logo">
  </div>
  <div>
    <div class="text-xl font-medium text-black">ChitChat</div>
    <p class="text-slate-500">You have a new message!</p>
  </div>
</div>
```
Tailwind’s flexbox and padding utilities (flex, shrink-0, and p-6) to control the overall card layout
The max-width and margin utilities (max-w-sm and mx-auto) to constrain the card width and center it horizontally
The background color, border radius, and box-shadow utilities (bg-white, rounded-xl, and shadow-lg) to style the card’s appearance
The width and height utilities (w-12 and h-12) to size the logo image
The space-between utilities (space-x-4) to handle the spacing between the logo and the text
The font size, text color, and font-weight utilities (text-xl, text-black, font-medium, etc.) to style the card text


## Links
* [Box Alignment Cheatsheet](https://rachelandrew.co.uk/css/cheatsheets/box-alignment)
* https://codepen.io/bradtraversy/pen/JgXqBL
* https://docs.mongodb.com/manual/tutorial/install-mongodb-on-os-x/
* https://caniuse.com/?search=focus-visible
* https://www.youtube.com/c/TailwindLabs
* [Caniuse](https://caniuse.com/)
* [Netflix Top 10](https://top10.netflix.com/films/2022-02-06)
* [Tailwind Play](https://play.tailwindcss.com/YelhilBeHb)


# 
* `flex` -  
* `items-center` -  align items along the center of the container’s cross axis
* `justify-between` - justify items along the container’s main axis such that there is an equal amount of space between each item.
* `py-6` - 
* border-gray-100 
* items-left 
* border-b-1 
* `md:justify-start` - mid breakpoint: to justify grid items against the start of their inline axis.
* md:space-x-10
* `max-w-7xl` - 
* `flex-col` - to stack things vertically
* `justify-end` to place card at the bottom of the screen
* `h-full` - add height to flex container
* `p-8` - add padding to separate elements from screen edge
* `space-y-4` - spacing utility
* `tracking-wider` - increase the letter spacing
* `absolute` -
* `relative` -
* `overflow-hodden` - prevent bleeding from the container
* use `grid` to center elements
* `grid-place-items-center` to center is vertically and horizontaly
* `object-cover` - this attribute prevents stretching of an image
* `class="grid place-items-center"` - to center elements on the viewport
* `justify-content` - 
#### When aligning items on the inline axis you will use the properties which begin with justify-:
  * justify-items
  * justify-self
  * justify-content
#### When aligning items on the block axis you will use the properties that begin align-:
* align-items
* align-self
* align-content

Flexbox adds an additional complication in that the above is true when flex-direction is set to row. The properties are swapped when flexbox is set to column. Therefore, when working with flexbox it is easier to think about the main and cross axis rather than inline and block. The justify- properties are always used to align on the main axis, the align- properties on the cross axis.

#### The alignment subject
The alignment subject is the thing that is being aligned. For justify-self or align-self, or when setting these values as a group with justify-items or align-items, this will be the margin box of the element that this property is being used on. The justify-content and align-content properties differ per layout method.

#### The alignment container
The [alignment container](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Box_Alignment) is the box the subject is being aligned inside. This will typically be the alignment subject's containing block. An alignment container may contain one or many alignment subjects.

#### Types of alignment
There are three different types of alignment that the specification details; these use keyword values.

Positional alignment: specifying the position of an alignment subject with relation to its alignment container.
Baseline alignment: These keywords define alignment as a relationship among the baselines of multiple alignment subjects within an alignment context.
Distributed alignment: These keywords define alignment as a distribution of space among alignment subjects.



## Building a Youtube thumbnail with Tailwindcss
```html
<body class="grid min-h-screen p-4 bg-gray-900 place-items-center">
    <div class="relative w-[640px] h-[360px] bg-white overflow-hidden">
        <!-- Top right circle -->
        <div aria-hidden="true" class="absolute -top-16 -left-12 w-[200px] h-[200px] bg-purple-500 rounded-full grid-place-items-center">
            <svg class="w-[64px] h-[72px] ml-3 mt-3" viewbox="0 0 64 72" fill="none" xmlns="http://www.w3.org/2000/svg"></svg>
        </div>
        <!-- Right big circle -->
        <div aria-hidden="true" class="absolute w-[512px] h-[512px] bg-purple-200 rounded-full -top-20 -right-56" ></div>
        <!-- Images -->
        <div class="absolute top-8 right-8">
          <img src="" alt="image" class="object-cover w-64 shadow-2xl h-36 rounded-2xl rotate-3"/>
          <img src="/img/Screen-shot-code.png" alt="Code" class="object-cover w-64 translate-x-16 shadow-2xl h-36 rounded-2xl -rotate-3"/>
        </div>
        <!-- Play button -->
        <div class="absolute inset-0 grid items-center right-12">
          <a href="#" class="grid w-12 h-12 transition bg-purple-500 rounded-full ring-white place-items-center hover:bg-purple-300">
            <span class="sr-only">Watch the video</span>
            <svg class="w-4 m-1" viewbox="0 0 16 18" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="#" fill="white"/>
            </svg>
          </a>
        </div>
        <!-- Content -->
        <div className="relative p-8 flex flex-col justify-end w-2/3 h-full space-y-4">
            <p class="text-xs font-semibold tracking-wider text-purple-600 uppercase">How to build this</p>
            <h1 class="text-4xl font-extrabold">Youtube thumbnail with Tailwind CSS</h1>
            <svg class="w-36" viewbox="0 0 145 19" fill="none" xmlns="http://www.w3.org/2000/svg"></svg>
        </div>
    </div>
</body>
```

## Glowing Effect with Blur filter
```javascript
<body className="min-h-screen px-8 py-16 bg-gray-700">
  <div className="grid gap-8 items-start justify-center">
    <button className="px-7 py-4 bg-black rounded-lg leading-none flex items-center">
      <span className="text-gray-100">Labs Release</span>
    </button>
  </div>
</body>


<div className="px-2 py-4 bg-black">
  <div className="grid items-start justify-center gap-8 mt-8">
    <div className="relative group">
      <div className="group-hover:opacity-100 transition duration-1000 group-hover:duraation-200 absolute rounded-lg opacity-80 bg-gradient-to-r from-pink-600 to-purple-500 -inset-3 blur-[2px] animate-tilt"></div>
      <button className="relative flex items-center py-4 leading-none bg-black rounded-lg px-4">
        <span className="pl-2 pr-2 text-gray-300 transition duration-300 group-hover:text-gray-100">Get started</span>
      </button>
    </div>
  </div>
</div>
```

## Borders
* 

* [Welcome to the Contentful help center](https://gifted-raman-ffba9b.netlify.app/)
* https://www.youtube.com/watch?v=ZZRTUpRzETo
* https://developer.mozilla.org/en-US/docs/Web/HTML/Element/header
