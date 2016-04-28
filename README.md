# envm

Environment variable management for each project. 

`envm` command is thin wrapper of `envdir`. This add a rule to store environment variables under `$HOME/.envm`.
For example, variables for the project in `/path/to/project` are saved in `$HOME/.envm/path/to/project/`.


## Usage

```
Usage:
  envm ls            - lists environment valiables
  envm exec COMMAND  - wraps COMMAND with envdir
  envm set KEY VALUE - sets environment valiables
  envm get KEY       - gets the value of KEY
  envm edit KEY      - edits with $EDITOR
  envm rm KEY        - removes the environment variable
  envm help          - shows this message
```

## LICENSE

MIT
