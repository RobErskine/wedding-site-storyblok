## Storyblok + Next.js Demo

This is the example repository for building a starter site with Storyblok + Next.js.

1. Clone down this repository.
2. Duplicate the [Next.js Boilerplate in Storyblok](https://app.storyblok.com/#/me/spaces/169726/dashboard). Name it something descriptive.
3. Duplicate the .env.example file in this repo and rename it to .env.local. Drop in your Storyblok API key from your duplicated space.
4. Install dependencies and start the development server `npm install && npm run dev`
5. Follow the instructions below for setting up a local ssl cert to get https working for localhost
6. local-ssl-proxy --source 3010 --target 3000 --cert localhost.pem --key localhost-key.pem

The last step will proxy https://localhost:3010 to http://localhost:3000

Lastly set up your default preview url in Storyblok to https:localhost:3010

## Setting up local ssl cert

If you haven't installed `mkcert` yet:

1. $ brew install mkcert
2. $ mkcert -install
3. In the root directory, run $mkcert localhost
4. $ npm install -g local-ssl-proxy
5. Run step 5 in the regular instructions 


## Learn More

To learn more about Next.js, take a look at the following resources:

- [Add a headless CMS to Next.js in 5 minutes](https://www.storyblok.com/tp/add-a-headless-cms-to-next-js-in-5-minutes) - Tutorial to get started with Next.js & Storyblok
- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.
