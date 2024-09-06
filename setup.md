Step 1: Run the following Commands

```
npm install -D tailwindcss
npx tailwindcss init

```

Step 2: Add these lines in tailwind.config.js

```
  content: ["./src/**/*.{html,js}"],

```
Step 3: Add these lines in src/input.css

```
@tailwind base;
@tailwind components;
@tailwind utilities;

```
Step 4: Run the following Command 

```
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch

```

Step 6: Add this line in package.json

```
"dev": "vite"

```

Step 5: Add this file in with html extention in src folder

```
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

