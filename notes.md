npm init -y  // this initializes package.json
npm i express  // installs express
npx gitignore node // initiates a gitignore file tailored for node
touch index.js 
in package.json, change the "scripts" section to say "start": "node index.js"  // this tells the system to look at index.js when the start script is invoked
set up index.js to start the server, indicate port, ect.
npm start // starts the server
npm i -D nodemon  // installs nodemon as a development dependency

push new code to github so heroku will have something to work with, not just an empty repo
create new app on heroku
connect to github
enable automatic depolyments on the specified branch

We need to make the port dynamic using an environment variable or heroku will still throw an error
const port = process.env.PORT || 4000;  // PORT is for heroku, 4000 is for local deployment

server.listen(port, () => console.log(`*** Server running on port ${port}! ***`));
