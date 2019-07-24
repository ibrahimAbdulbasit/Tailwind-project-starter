# you can just pull this repo and do
`npm install`

# or you can do it your self
- Tailwwind is a package available in npm so you can start by creating a packge.json file do:
    `npm init -y`
- you need to install tawilwindcss and postcss-cli and autoprefixer
    `npm install tailwondcss postcss-cli autoprefixer`
- now you need to configure tailwind by creating a tailwind.config.js file using:
    `npx tailwind init`
- then you need to configure postcss by creating a postcss.config.js file thats include the plugins you want to use require('tailwindcss), require(autoprefixer).
- then you create a css file so that tailwind can look into it and create your fianl css based on it
    - in it define @tailwind base; @tailwind components; @tailwind utilities;
- then wirte a script on the package.json file to proces the work
    `postcss css/tailwind.css -o pubilc/build/tailwind.css`