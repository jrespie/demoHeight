# Demo Height app

This exists to demonstrate how apps appear differently on mobile simulators vs real mobile devices

# Instructions

Clone this repo

Install dependencies by:
> npm i

Start the app by:
> npm start

Browse to
> http://localhost:3000

to see the app in your browser

# To view on mobile device

The easiest way to view on a mobile device is via ngrok.
Which means [signing up for, and installing, ngrok](https://ngrok.com/).

Once installed, you can run
> ./ngrok http localhost:3000

This will give you a URL that you can then browse to from any device, that will point to your local running instance.

# The problem

The problem lies in the use of 'vh' for the parent div.
You can see it in the CSS [here](https://github.com/jrespie/demoHeight/blob/61b6857ef0f2d946f06471378480093add5d6068/public/stylesheets/style.css#L12)

Try changing this to 100% instead, and you should see the problem resolved!
