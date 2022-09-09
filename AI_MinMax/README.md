If you would like to run this code, there are a set of steps you need to follow. First, Make sure you have Node.js installed on your system.

These instructions are for Windows machines, please use the appropriate Linux/Unix commands when appropriate or see https://poke-env.readthedocs.io/en/stable/getting_started.html for help

Now go to your command line: git clone https://github.com/ArcadeRaven/CSC540---pokemon-showdown cd CSC540---pokemon-showdown npm install

There will be a few vulnerabilities, this is from the API's use of Node.js. To bypass, create a lockfile using this command: npm i --package-lock-only

Now run this: npm audit fix --force

You may need to run npm audit fix --force 1 or 2 more times.

cd config copy config-example.js config.js

Here you should see it return "1 file(s) copied."

Finally, you are done with the one-time installs. Now every time you want to run the server, simply cd to where you installed CSC540---pokemon-showdown and run: node pokemon-showdown start --no-security

Go to the localhost address and run all of the cells in MinMax.ipynb In the host site, you can view the battles and the compiler will return the win rate.

Press Ctrl + C to stop the server.
