# Tailwind intial setup

Let's do the basic tailwind hello world.

```bash
# create folder
mkdir 01-initial-setup
cd 01-initial-setup
# setup package.json, you can just confirm everything
npm init
# install and init tailwind
npm install -D tailwindcss
npx tailwindcss init
```

Configure content path in tailwind config
```js
/* tailwind.config.js */
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

Create css file and add tailwind directives
```css
/* src/input.css */
@tailwind base;
@tailwind components;
@tailwind utilities;
```

Start tailwind build and watch, optionaly add below prompt to package.json scripts
```bash
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
```

Use tailwind in html, test in liveserver
```html
<!-- src/index.html -->
<!doctype html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="./output.css" rel="stylesheet">
</head>
<body>
  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>
</body>
</html>
```