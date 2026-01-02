## Fix/ Installation project Flower-web-page

### Add the file tailwind.config. (current project)

> N.B: when not generated first installing the package tailwindcss in the project

You can create the **tailwind.config.js** file using the Tailwind CSS CLI or by **manually** creating the file in your project's root directory.

#### Method 1: Using the Tailwind CLI (Recommended)

The easiest way to generate the configuration file is to use the init command provided by the Tailwind CSS package.

1. Open your terminal in the root directory of your project.

<br/>

2. Run the following command to generate a minimal tailwind.config.js file:

> npx tailwindcss init

To also generate a postcss.config.js file, add the -p (for PostCSS) flag:

> npx tailwindcss init -p

<br/>

3. A tailwind.config.js file will be created in your root directory. Tailwind CSS automatically uses this file if it's in the default location.

<br/>

**Core Problem:** how to integrate properly **tailwind.config.js** right at the installation of **tailwindCss** package inside your new project ?
