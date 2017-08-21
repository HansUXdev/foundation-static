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
└─── src
│   └─── assets
│   └─── img
│   └─── js
│     └─── building-blocks
│     └─── components
│     └─── lib
│   └─── scss
│     └─── building-blocks
│     └─── components
│     app.scss
│     _settings.scss
│     _block-settings.scss
│   └─── partials
│        └─── building-blocks
└─── Publics
│   └─── ... // built from the gulpfile  
└─── views
│   │ index.handlebars
│   │ login.handlebars
│   │ register.handlebars
│   └─── admin
│     └─── admin.handlebars
│     └─── ... *.handlebars
│   └─── layouts
│       └─── main.handlebars
│       └─── dashboard.handlebars
│       └─── offcanvas.handlebars
│       └─── sidebar-left.handlebars
│   └─── partials
│        ... *.handlebars
│        └─── building-blocks
└─── models
│   └─── mongoose   // mongoose schemas 
│   └─── sequelize  // sequelize schemas
└─── controllers
│   │   admin.js
│   │   home.js
│   │   errors.js
│   │   sessions.js
```
