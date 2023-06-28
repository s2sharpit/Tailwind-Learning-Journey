- `npm init -y`          // This initializes the directory as a Node.js project
- `npm install -D tailwindcss postcss autoprefixer vite`          // installs required packages
- `npx tailwindcss init -p`
- In your `tailwindcss.config.js` file replace `content: []`, with `content: ["*"]`
- Create a CSS file named `style.css`, add it to your HTML, and edit it with the following content:

    ```css
    @tailwind base;
    
    @tailwind components;
    
    @tailwind utilities;
    ```

- Link the CSS file with `"./style.css"` in the `href` attribute.

### To start the server

- Add `"start": "vite"` to the scripts in your `package.json`
- Run the command `npm run start` to start a development server

### To extend the Tailwind CSS configuration

- Run `npx tailwindcss init confTailcss --full`

### To deploy the Tailwind website to production

- Add `"build": "vite build"` to the scripts in your `package.json`
- To start the build server, run `npm run build`
- In `dist/index.html`, add `.` before `"/assets"` where the CSS file is linked.

### To create and use a template file

- First, set up Tailwind CSS
- Copy the folder with the template
- Delete the `node_modules` file
- Run the command `npm i`
