By convention, create a `bin` directory to hold the actual command.

Add the script you want to run in your cli in the bin key insdie `package.json`.

Run `npm link .` so it can be invoked from the command line on your machine. However, instead of being installed directly from the npm repository, the install is linked to our project. This means we can continue to build out our project and still be able to invoke it from the command prompt/line. You can also run `npm unlink` to unlink/remove the script from the command line

### Popular Configuration File Formats
| Format        | Examples           |
| ------------- |:-------------:|
| ini           | Git config, Pypi config, AWS credentials |
| json          | Visual Studio Code settings, Yeoman config      |
| XML           | Maven settings, NuGet config      |

JSON allows the user to override specific JSON properties with their own configuration values.
No matter the format, settings are scoped to the individual user by storing int the user's home directory. Often prefixed with a "dot" or in a directory prefixed with a "dot". This is because the `ls` command by default, will skip files and directories that begin with a dot, so as not to clutter the user's view of the application system.

```
Find out where the config is stored on mac when using configstore???
```

Secure secrets
Using `keytar` can help securely store secrets in a user's device irrespective of the OS.
