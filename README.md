# Next Saas AI Application

Next.js application for Saas AI Platform using Next.js, React, Tailwind, Prisma, Planetscale, MySQL & Stripe.

use [Stripe Testing Cards](https://stripe.com/docs/testing)

## Features

- Tailwind CSS with Shadcn UI
- Clerk Authentication
- Client form using react-hook-form
- Server error handling using react-toast
- Conversation Generation Tool (Open AI)
- Image Generation Tool (Open AI)
- Video Generation Tool (Replicate AI)
- Music Generation Tool (Replicate AI)
- Stripe monthly subscription
- Free tier with API limiting
- Stripe webhooks
- MySQL + Prisma + PlanetScale

## Installation

**Node version 18.x.x**

### Cloning the repository

```shell
git clone https://github.com/nrocchi/next-saas-ai-app.git
```

### Install packages

```shell
npm i
```

### Setup .env file


```js
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/dashboard
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/dashboard

OPENAI_API_KEY=
REPLICATE_API_TOKEN=

DATABASE_URL=

STRIPE_API_KEY=
STRIPE_WEBHOOK_SECRET=

NEXT_PUBLIC_APP_URL="http://localhost:3000"
```

### Setup Prisma

Add MySQL Database (I used PlanetScale)

```shell
npx prisma generate
npx prisma db push
```

### Start the app

```shell
npm run dev
```

## Available commands

Running commands with npm `npm run [command]`

| command         | description                              |
| :-------------- | :--------------------------------------- |
| `dev`           | Starts a development instance of the app |

## Contributors

The original author is [Nicolas Rocchi](https://github.com/nrocchi).
