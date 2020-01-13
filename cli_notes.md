By convention, create a `bin` directory to hold the actual command.

Add the script you want to run in your cli in the bin key insdie `package.json`.

Run `npm link` so it can be invoked from the command line on your machine. However, instead of being installed directly from the npm repository, the install is linked to our project. This means we can continue to build out our project and still be able to invoke it from the command prompt/line. You can also run `npm unlink` to unlink/remove the script from the command line
