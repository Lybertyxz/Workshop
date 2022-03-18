<div id="top"></div>

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a>
    <img src="https://miro.medium.com/max/312/0*Z-jwqyt2k8NbHaQe.png" alt="Logo">
    <img src="https://laravel.sillo.org/wp-content/uploads/2021/04/Capture.png" alt="Logo">
  </a>

  <h3 align="center">WORKSHOP FRAMER MOTION / TAILWIND CSS</h3>

  <p align="center">
    You will learn how to create awesome animations and beautiful pages in NextJS
    <br />
    <a href="https://tailwindcss.com/docs/"><strong>Explore the docs (TailwindCSS)</strong></a>
    <br />
    <a href="https://www.framer.com/docs/"><strong>Explore the docs (FramerMotion)</strong></a>
    <br />
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#exercices">Exercices</a></li>
  </ol>
</details>

<!-- GETTING STARTED -->
## Getting Started

### Installation

Below is an example of how you can install and set up the Workshop.
  
1. Make sure you have Node installed either follow the step on this link [NodeJS](https://nodejs.org/en/download/package-manager/)

2. Create a new NextJs project
   ```sh
   npx create-next-app my-project
   ```

3. Install TailwindCSS
   ```sh
   npm install -D tailwindcss postcss autoprefixer --save
   npx tailwindcss init -p
   ```

4. Add the paths to all of your template files in your tailwind.config.js file.
   ```sh
   module.exports = {
    content: [
      "./pages/**/*.{js,ts,jsx,tsx}",
      "./components/**/*.{js,ts,jsx,tsx}",
    ],
    theme: {
      extend: {},
    },
    plugins: [],
    }
   ```

5. Add the @tailwind directives for each of Tailwind’s layers to your ./styles/globals.css file.
    ```sh
        @tailwind base;
        @tailwind components;
        @tailwind utilities;
    ```

6. Install FramerMotion dependencies
    ```sh
        npm i framer-motion --save
    ```

6. You're all set ! Run the project by using :
    ```sh
        npm run dev
    ```

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- USAGE EXAMPLES -->
## Exercices

1. Clean the pages/index.js file like so
    ```sh
    import Header from "../components/Header"

    export default function Home() {
      return (
        <div>
          <Header/>
        </div>
      )
    }
    ```

2. Create a Header component in a new folder components : /components/Header.js
    ```sh
    import { motion } from "framer-motion"

    export default function Header () {
        return (
            <motion.div>
            </motion.div>
        )
    }
    ```

3. Now use the docs to create the header with 3 navigation buttons and one logo

<p align="right">(<a href="#top">back to top</a>)</p>
