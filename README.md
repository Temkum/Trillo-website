# Trillo Web App

Built with Flexbox

Run `npm install`
then `npm run start`

**Paste in json later:**
"devserver": "live-server",
"start": "npm-run-all --parallel devserver watch:sass",
"compile:sass": "node-sass sass/main.scss css/style.comp.css",
"prefix:css": "postcss --use autoprefixer -b 'last 10 versions' css/style.comp.css -o css/style.prefix.css",
"compress:css": "node-sass css/style.prefix.css css/style.css --output-style compressed",
"build:css": "npm-run-all compile:sass prefix:css compress:css"