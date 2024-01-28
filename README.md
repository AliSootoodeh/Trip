## Create Next App

```sh
npx create-next-app@latest appName

```

## Libraries

```sh
npm install @clerk/nextjs@4.26.1 @prisma/client@5.5.2 @tanstack/react-query@5.8.1 @tanstack/react-query-devtools@5.8.1 axios@1.6.1  openai@4.14.2   react-hot-toast@2.4.1 react-icons@4.11.0
```

```sh
npm install -D @tailwindcss/typography@0.5.10  daisyui@3.9.4 prisma@5.5.2
```

## DaisyUI

- remove default code from globals.css
  tailwind.config.js

```js
{
plugins: [require('@tailwindcss/typography'), require('daisyui')],
}
```

## Deploy

package.json

```js

"scripts": {
    "build": "npx prisma generate && next build",
  },
```

- Neon DB
- github repo
- vercel
- envirment variables

```js

"env": {
    "DATABASE_URL": "",
    "NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY":"",
    "CLERK_SECRET_KEY":""
    "OPENAI_API_KEY":""
    "UNSPLASH_API_KEY":""
  },
```
