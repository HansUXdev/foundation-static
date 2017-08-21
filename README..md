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
│   │    └─── img
│   │    └─── js
│		│				└─── building-blocks
│		│				└─── components
│		│				└─── lib
│		│				└─── app.js
│   │    └─── scss
│		│				└─── building-blocks
│		│				└─── components
│		│				└─── app.scss
│		│				└─── _settings.scss
│		│				└─── _block-settings.scss // gulp made
│   └─── partials
│        └─── building-blocks
└─── Publics
│   └─── ... // built from the gulpfile  
└─── views
│   │   index.handlebars
│   │   login.handlebars
│   │   register.handlebars
│   └─── assets
│   │    └─── img
│   │    └─── js
│		│				└─── building-blocks
│		│				└─── components
│		│				└─── lib
│		│				└─── app.js
│   │    └─── scss
│		│				└─── building-blocks
│		│				└─── components
│		│				└─── app.scss
│		│				└─── _settings.scss
│		│				└─── _block-settings.scss // gulp made
└─── models
│   └─── mongoose     // mongoose schemas 
│   └─── sequelize		// sequelize schemas
└─── controllers
│   │   admin.js
│   │   home.js
│   │   errors.js
│   │   sessions.js
```