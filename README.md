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
* `space-y-2` - vertical spacing utility.  Use it when 

### Nesting
```html
<body class="bg-gray-100">
    <div class="px-8 py-12">
      <img class="h-10" src="/img/logo.svg" alt="Workcation" />
      <img
        class="mt-6 rounded-lg shadow-xl"
        src="/img/beach-work.jpg"
        alt="Woman workcationing on the beach"
      />
      <h1 class="mt-6 text-2xl font-bold text-gray-900">
        You can work from anywhere.
        <span class="text-indigo-500">Take advantage of it.</span>
      </h1>
      <p class="mt-2 text-gray-600">
        Workcation helps you find work-friendly rentals in beautiful locations so you can enjoy some
        nice weather even when you're not on vacation.
      </p>
      <div class="mt-4">
        <a
          class="inline-block px-5 py-3 text-sm font-semibold tracking-wider text-white uppercase bg-indigo-500 rounded-lg shadow-lg"
          href="#"
        >
          Book your escape
        </a>
      </div>
    </div>
  </body>
```

## Commands
* `npx tailwindcss -o build.css --minify`
* `npx tailwindcss-cli build tailwind.css -o build/tailwind.css`
* `npm init -y`
* `npm install -D tailwindcss postcss autoprefixer vite`
* `npx tailwindcss init -p`

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
