---
sidebar_position: 1
---

# Getting Started

Jumpstart UI uses **tailwindcss** and **@headlessui/react** for it’s components, so it is recommended that you have tailwind installed(not necessary).

## Installation

To install jumpstart create a new react app(using any framework of your choice). 

### Prerequisites

Jumpstart UI uses **tailwindcss** and **@headlessui/react** for it’s components, so it is recommended that you have tailwind installed(not necessary).


```shell
yarn create next-app myCoolApp
```

<!-- You can follow the official tailwind **[installtion guide](https://tailwindcss.com/docs/installation)**. -->


```shell title="Install Tailwind, Headless UI and Heroicons"
yarn add tailwindcss@latest postcss@latest autoprefixer@latest @headlessui/react @heroicons/react --D
```
```shell title="Create your configuration files"
npx tailwindcss init -p
```

Replace purge empty array with 

```js title="tailwind.config.js"
['./pages/**/*.{js,ts,jsx,tsx}', './components/**/*.{js,ts,jsx,tsx}'],
```

Remove all existing code in `./styles/globals.css` and paste this code, delete `./styles/Home.modules.css`

```css title="./styles/globals.css"
@tailwind base;
@tailwind components;
@tailwind utilities;
```

### Installation

```shell
yarn add jumpstart-ui
```
