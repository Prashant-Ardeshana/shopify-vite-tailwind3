# Magic Theme test

## Overview
The Base Theme is a Shopify theme development setup that leverages modern tools such as Vite, TailwindCSS, and the Shopify CLI to streamline the development process. It allows for efficient local development, hot-reloading, and easy deployment to the Shopify store.

### Install in the other themes.
Follow this blog.
[How to setup Shopify Vite with Tailwind CSS.](https://dev.to/prashant-ardeshana/how-to-setup-shopify-vite-with-tailwind-css-3fga)

## Dependencies
Ensure you have the following dependencies installed before setting up the theme:
- [Shopify CLI](https://shopify.dev/docs/themes/tools/cli) Shopify's command-line tool for managing themes.
- [TailwindCSS](https://tailwindcss.com/) Utility-first CSS framework.
- [Vite](https://vitejs.dev/guide/) Next-generation frontend tooling.
- [Shopify Vite Plugin](https://shopify-vite.barrelny.com/) Plugin to integrate Vite with Shopify themes.

## Setup
We are using the Vite Plugin for Shopify. [Learn more here.](https://shopify-vite.barrelny.com/guide/)

### First time setup

Clone the repository:
```
git clone https://github.com/your-repo/base-theme.git
cd base-theme
```

Install dependencies:
```
npm install
```

### Local Devlopment

Run dev server with hot reload (accepts all [theme commands](https://shopify.dev/docs/api/shopify-cli/theme/theme-push)):
```
npm run dev -- --store StoreName --live-reload hot-reload
```

This will run both `shopify theme dev` and `vite:dev` to start the shopify server and vite compilation.


### Deployment

To deploy the theme store as a new theme (without pushing to live), run:
```
npm run deploy -- --store StoreName 
```
Deploy theme store as new theme. Accepts all `shopify theme push` commands and does _not_ allow pushing to live. 

## Best Practices
Use Git for version control: Commit changes frequently and use branches for new features.

Follow Shopify theme development guidelines: Adhere to Shopify's theme development best practices.

Keep dependencies updated: Regularly update npm packages for security and performance improvements.

Use TailwindCSS efficiently: Keep styles modular and avoid excessive custom CSS.

## Troubleshooting

### Common Issues & Fixes
Command not found: Ensure you have Shopify CLI and Node.js installed.

Live reload not working: Restart the dev server and check for browser console errors.

Deployment failure: Ensure your Shopify store permissions allow theme deployment.

## Contribution
We welcome contributions! Feel free to submit a pull request or open an issue to suggest improvements.


## License
This project is licensed under the MIT License.
