# Foundation-Static
This is a Express.js fork of the classic [Zurb Template](https://github.com/zurb/foundation-zurb-template/). It takes advantage of the most advanced front-end framework by allowing you to utilize [Building Blocks](foundation.zurb.com/building-blocks/). That way you can spend less time reinventing the wheel and more time prototyping, customizing/theming and building out the backend. 

Here is the [live](https://foundation-static.herokuapp.com/#) link.

## Requirements
- node and npm installed
- nodemon installed
- sass installed (?)
- [foundation cli](https://github.com/zurb/foundation-cli) is recommended to be installed to take full advantage of front-end components
- [heroko cli](https://devcenter.heroku.com/articles/heroku-cli) is recommended to be install


## Try it out and let me know what you think.
- Clone, Fork or download the project
- Install everything ```npm i```
- Start the project ```npm run start```
- Install a new component ```foundation blocks install foundation-5-top-bar```
- Commit to your own repo ```npm run git```
- Deploy to Heroku ```heroku login``` then ```heroku create``` then whenever you need to push changes to the live site, ```npm run heroku```
- Its that easy.

## Why did I make this? 
Because I wanted a super lightweight MODERN server that is easy to learn, teach and use for projects.

## Goals
- LIGHT weight node server
- Amazingly fast front-end prototyping using [Building Blocks Compatable !](http://foundation.zurb.com/building-blocks/) to build production ready sites in hours not days and progressively build the backend as needed.
- Deploy to Heroku

## Features
- [Building Blocks Compatable !](http://foundation.zurb.com/building-blocks/)
- [Templates !](http://foundation.zurb.com/templates.html)
  - Because it makes life easier and they should be in the [Zurb Template](https://github.com/zurb/foundation-zurb-template/)...
- Handlebars HTML templates with Express
- Sass compilation and prefixing
- JavaScript module bundling with webpack
- Built-in BrowserSync/Nodemon server 
  - run nodemon ./server.js localhost 8080
- For production builds:
  - CSS compression
  - JavaScript compression
  - Image compression
- Automatic Responsive Testing via [Nightmare](https://github.com/segmentio/nightmare)
	- Just run ```node browser-tests.js```

## Future Goals
- firebase components for plug and chug back-end
- Incorporated into [Zurb Foundation's CLI](https://github.com/zurb/foundation-cli) as an alternitive to static site prototypes.

# File Structure
```
project root
│   README.md
│   config.yml 
│   gulpfile.babel.js
│   nodemon.json
│   Procfile
│   server.js
│   ...
│   // Installing components aka building-blocks is easy
│   // EX:foundation blocks install table-expand
│   // Will add the file to js/building-blocks/ & scss/building-blocks/ & partials/building-blocks/
│   // then app.js & app.scss will automatically be updated to include the component
│   // gulp will then copy src/partials/building-blocks/ to view/block/ 
│   // then compile everything else to ./public/
└─── src/
│   └─── data/
│        ... // where .js files go for static prototyping data
│   └─── partials/
│     └─── building-blocks
│   └─── assets/
│     └─── img/
│     └─── js/
│       └─── building-blocks/
│       └─── components/
│       └─── lib/
│     └─── scss/
│       └─── building-blocks/
│       └─── components/
└─── Publics/
│   └─── ... // built from the gulpfile  
└─── views/
│   │ index.handlebars
│   │ login.handlebars
│   │ register.handlebars
│   └─── admin/
│     └─── admin.handlebars
│     └─── ... *.handlebars
│   └─── layouts/
│       └─── main.handlebars
│       └─── dashboard.handlebars
│       └─── offcanvas.handlebars
│       └─── sidebar-left.handlebars
│   └─── partials
│        ... *.handlebars
│        └─── building-blocks/
└─── models/
│   └─── mongoose/   // mongoose schemas 
│   └─── sequelize/  // sequelize schemas
└─── controllers/
│     └─── admin.js
│     └─── home.js
│     └─── errors.js
│     └─── sessions.js
```
