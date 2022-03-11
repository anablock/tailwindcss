# README

* `class="md:flex"` - 

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
* `uppercase` - 
* When using uppercase, increase letter spacing by using `tracking-wider` and `font-semibold`
* `relative` - 
* `flex` - Utilities for controlling how flex items both grow and shrink.
* `items` - Utilities for controlling how flex and grid items are positioned along a container's cross axis.
* Use justify-between to justify items along the container’s main axis such that there is an equal amount of space between each item

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

## Building a Youtube thumbnail with Tailwindcss
```html
<body class="grid min-h-screen p-4 bg-gray-900 place-items-center">
    <div class="w-[640px] h-[360px] bg-white">
        <!-- Top right circle -->
        <!-- Right big circle -->
        <!-- Images -->
        <!-- Play button -->
        <!-- Content -->
        <div class="flex flex-col justify-end w-2/3 h-full space-y-4">
            <p class="text-xs font-semibold tracking-wider text-purple-600 uppercase">How to build this</p>
            <h1 class="text-4xl font-extrabold">Youtube thumbnail with Tailwind CSS</h1>
            <svg class="w-36" viewbox="0 0 145 19" fill="none" xmlns="http://www.w3.org/2000/svg"></svg>
        </div>
    </div>
</body>
```