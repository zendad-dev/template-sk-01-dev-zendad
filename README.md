# template-sk-01-dev-zendad
This repository --01 ... contains the initial Sveltekit skeleton project setup with answers to Yes for Eslint, Typescript, Prettier, and Playwright. That's just the first step.  There are several others, listed below, until the template is complete.

To summarize:
1.  Create Sveltekit Project
2.  Add TailwindCSS
3.  Add Prettier plugin for TailwindCSS (necessites the removal of the default Prettier Plugin Svelte)
4.  Add Node adapter
5.  Add Lib directory and other standard Project files

-------

1.  From https://kit.svelte.dev/docs/introduction#before-we-begin:
npm create svelte@latest my-app
cd my-app
npm install

2.  From https://tailwindcss.com/docs/guides/sveltekit:
npm install -D tailwindcss postcss autoprefixer svelte-preprocess
npx tailwindcss init tailwind.config.cjs -p

3a.  From https://github.com/tailwindlabs/prettier-plugin-tailwindcss:
npm install -D prettier prettier-plugin-tailwindcss
Create prettier-config.js in the root of the project directory and add the following code:

// prettier.config.js
module.exports = {
  plugins: [require('prettier-plugin-tailwindcss')],
}

- or - From https://stackoverflow.com/questions/63266052/vscode-change-vertical-guide-line-indentation/69124944#69124944: 

module.exports = {
    tabWidth: 4,
    tabs: true,
    // other options...
}

3b. Remove default Prettier Plugin Svelte
npm uninstall prettier-plugin-svelte

4.  From https://www.npmjs.com/package/@sveltejs/adapter-node:
npm i -D @sveltejs/adapter-node
change svelte-config.js auto to node, follow other instructions. 

5.  From https://kit.svelte.dev/docs/project-structure and from https://tailwindcss.com/docs/guides/sveltekit:
Add Lib directory 
Add __layout.svelte
etc....
