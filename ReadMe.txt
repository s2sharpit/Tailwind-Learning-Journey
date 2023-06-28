- npm init -y          // This initializes the directory as a NodeJs project
- npm install -D tailwindcss postcss autoprefixer vite          // installs required packages
- npx tailwindcss init -p
- In your tailwindcss.config.js file replace content:[], with content: ["*”]
- Create a css file “style.css”, add it to your html and edit it with this content:
    
    @tailwind base;
    
    @tailwind components;
    
    @tailwind utilites;
    
- link css file with “./style.css” in href.

### To start server

- Add “start” : “vite” to your scripts in package.json
- Add “npm run start” command to start a dev server


### To extend config of tailwindcss

- npx tailwindcss init confTailcss —full

### To deploy tailwind website to Production

- Add “build” : “vite build” to your scripts in package.json
- To start build server “npm run build”
- In dist - index.html add “.” before “/assets” where css file is linked.

### To create and use template file

- First setup the tailwindcss
- Copy the folder with Template
- Delete node_modules file
- run command “npm i”