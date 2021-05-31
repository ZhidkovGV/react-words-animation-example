This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Description

This repo provides example of animtion for some words in text using React

In this example both text and dictinary of animated words are constants, but in real world solution it's better to create separte component which will consume text and dictionary as props.

Benefits of this approach:
- No need to manually find indexes for words, all words in dictionary will animate
- Easy to re-use, you just need to pass different text and dictionary if needed
- Uses css animation, so performance shouldn't be damaged by this

Problems:
- if you have multiple occurancies of word and want to animate only one of them you'll need to develop additional code to solve this or move to using constant indexes instead of dictionary
