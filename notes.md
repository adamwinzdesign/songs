npm init -y  // this initializes package.json
npm i express  // installs express
npx gitignore node // initiates a gitignore file tailored for node
touch index.js 
in package.json, change the "scripts" section to say "start": "node index.js"  // this tells the system to look at index.js when the start script is invoked
set up index.js to start the server, indicate port, ect.
npm start // starts the server
npm i -D nodemon  // installs nodemon as a development dependency

create new app on heroku