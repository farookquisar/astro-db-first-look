DB: https://studio.astro.build/farookquisar/astro-db-first-look

--############################################################################################################

## ASTRO DB Usage

### 1. Create a DB in https://studio.astro.build/ (Create from Git)

    - Check the the **Action** Tab in Git project

### 2. Connect to the DB (to Astro Studio)

    `npm run astro login`

    `npm run astro link`

### 3. Run remote db from dev

1. Add **"dev-db": "astro dev --remote",** (in package.json)
2. Run the below command
   `npm run dev-db`

### 4. Build and Deploy (eg. Netlify)

1. Generate a token in Astro Studio
   - Go to the studio project (eg https://studio.astro.build/farookquisar/astro-db-first-look/data/Link)
   - Go to Settings -> Tokens -> Generate Token -> Copy the token (Give any name)
   - Go to netlify site and add an environment variable called "ASTRO_STUDIO_APP_TOKEN" and paste the token value generated
   - Add the below in package.json:
     **"build": "astro check && astro build --remote",**

# --############################################################################################################

# Astro Starter Kit: Minimal

```sh
npm create astro@latest -- --template minimal
```

[![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/withastro/astro/tree/latest/examples/minimal)
[![Open with CodeSandbox](https://assets.codesandbox.io/github/button-edit-lime.svg)](https://codesandbox.io/p/sandbox/github/withastro/astro/tree/latest/examples/minimal)
[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/withastro/astro?devcontainer_path=.devcontainer/minimal/devcontainer.json)

> 🧑‍🚀 **Seasoned astronaut?** Delete this file. Have fun!

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── public/
├── src/
│   └── pages/
│       └── index.astro
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

Any static assets, like images, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).
