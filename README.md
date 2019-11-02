# GoBarber

A simple project to barber shop manager.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development purposes.

<h3>Prerequisites</h3>

<h4>NodeJS</h4>

You need to install NodeJS on your computer before you can use "**GoBarber**". You can install NodeJS by following <a href="https://nodejs.org/en/download/package-manager/">these instructions</a>.

Once you have completed the installation process, try typing **```npm -v```** into your command line. You should get a response with the version of NodeJS.

<h4>Yarn</h4>

Once you have NodeJs instaled, you need to install Yarn. You can install Yarn by following <a href="https://yarnpkg.com/en/docs/getting-started">these instructions</a>.

After instalition, try typing **```yarn -v```** into your command line. You should get a response with the version of Yarn.

<h4>Docker</h4>

You need to install Docker on your computer before you can use "**GoBarber**". You can install Docker by following <a href="https://www.docker.com/get-started">these instructions</a>.

Once you have completed the installation process, try typing **```docker -v```** into your command line. You should get a response with the version of Docker.

If you are using Linux distributions, is recommended following <a href="https://docs.docker.com/install/linux/linux-postinstall/">these instructions</a> to manage Docker as a non-root use.

<h4>PostgreSQL</h4>

You need to configure PostgreSQL on your computer before you can use "**GoBarber**". You can configure PostgreSQL by following <a href="https://hub.docker.com/_/postgres">these instructions</a>.

<h4>MongoDB local or Atlas</h4>

You need to install and configure a MongoDB on your computer or have a connection string for a database in Atlas cloud.

You can install MongoDB by following these instructions (<a href="https://treehouse.github.io/installation-guides/mac/mongo-mac.html">Mac</a> and <a href="https://treehouse.github.io/installation-guides/windows/mongo-windows.html">Windows</a>).

<h4>Redis</h4>

You need to configure Redis on your computer before you can use "**GoBarber**". You can configure Redis by following <a href="https://hub.docker.com/_/redis">these instructions</a>.

<h4>REST API Client</h4>

Finally, you will need a rest api client to test "**GoBarber**". Examples:

<ul>
  <li><a href="https://insomnia.rest/">Insomnia</a></li>
  <li><a href="https://www.getpostman.com/">Postman</a></li>
  <li><a href="https://install.advancedrestclient.com/install">Advanced REST Client</a></li>
</ul>

It is recommended to install the extension ESLint and edit the REST Api Client' settings:
```
  "files.eol": "\n",
  "eslint.autoFixOnSave": true,
  "eslint.validate": [
    {
      "language": "javascript",
      "autoFix": true
    },
    {
      "language": "javascriptreact",
      "autoFix": true
    },
    {
      "language": "typescript",
      "autoFix": true
    },
    {
      "language": "typescriptreact",
      "autoFix": true
    }
  ]
```

## Deploy

After clone repository, go to folder and follow this steps:

- Run **`yarn`** to install dependencies;
- Create a **postgres** database;
- Create a **mongo** database;
- Create a **redis** database;
- Create a file **`.env`** based on the file **`.env.example`**;
- Put your credentials inside **`.env`**;
- Run **`yarn sequelize db:migrate`** to creat the migrations;
- Run **`yarn sequelize db:seed:all`** to creat the seed;
- Run **`yarn dev`** to start de aplication;
- Run **`yarn queue`** in another terminal to start de queue.

Now you can use your REST API Client to test "**GoBarber**".

## Built With

<ul>
  <li>NodeJS</li>
  <li>Docker</li>
  <li>PostgreSQL</li>
  <li>Mailtrap.io</li>
  <li>Redis</li>
  <li>Sentry.io</li>
</ul>

## Tools

<ul>
  <li>Sucrase + Nodemon;</li>
  <li>ESLint + Prettier + EditorConfig;</li>
  <li>Sequelize</li>
</ul>

## Authors

<ul>
  <li>Matheus Leandro</li>
</ul>

## License

This project is licensed under the MIT License - see the <a href="https://github.com/matheusleandroo/gobarber/blob/master/LICENSE">LICENSE.md</a> file for details.

Based on <a href="https://rocketseat.com.br/bootcamp">Rocketseat Bootcamp</a> :rocket:
