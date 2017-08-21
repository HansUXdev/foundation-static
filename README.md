# foundation-static
An Express.js fork of the classic Zurb Template.

# Features

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
