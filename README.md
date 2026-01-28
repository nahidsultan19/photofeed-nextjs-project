This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.js`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.

## project info

This is a simple Next.js project built primarily to explore and understand advanced routing features in the Next.js App Router. The main focus of the project is on implementing Parallel Routes and Intercepting Routes.

Parallel Routes are used to render multiple UI segments simultaneously within the same layout. This allows different parts of the page to load independently while sharing a common layout structure.

Intercepting Routes are used to override navigation behavior and display content in a different context without fully navigating away from the current page. In this project, intercepting routes are defined using the (.)[routeName] convention. This pattern enables us to intercept navigation to a specific route and render it inside a modal instead of performing a full page transition.

For example, when a user clicks on a photo, the application uses an intercepting route based on the photoID to display the photo details inside a modal overlay. At the same time, the URL updates correctly, and if the page is refreshed, the full photo page is rendered normally. This provides a seamless user experience similar to modern gallery applications.

In addition to routing features, I also implemented a custom API using Next.js Route Handlers. The API is responsible for handling photo data retrieval, allowing the frontend to fetch and display dynamic content. This demonstrates how Next.js can be used to build both the frontend interface and backend API within a single full-stack application.
