# envm

Environment variable management for each project. 


## What is this for?

Putting aside the question whether we should configure applications with environment variable,
I couldn't have found the acceptable way of managing them.
Writing environment variables in ~/.bashrc is the easiest, but inconvenient especially when you are working with many applications of different configurations.
Passing from command line is painful when you have many configuration key.
Using `envdir` of daemontools or preparing some scripts like `env.sh` is almost enough, but I have made some mistakes to push it to remote repository. `.gitignore` or `.git/info/exclude` are cumbersome for me. So I wrote this. Maybe it's a little like `heroku config`.

This `envm` command is thin wrapper of `envdir`. This add a rule to store environment variables under `$HOME/.envm`.
For example, variables for the project in `/path/to/project` are saved in `$HOME/.envm/path/to/project/`.


## Usage

```
Usage:
  envm ls            - lists environment valiables
  envm exec COMMAND  - wraps COMMAND with envdir
  envm set KEY VALUE - sets environment valiables
  envm edit KEY      - edits with
  envm rm KEY        - removes the environment variable
  envm help          - shows this message
```

## LICENSE

MIT

