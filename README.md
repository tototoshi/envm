# envm

Environment variable management for each project. 

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

```
$ cd /path/to/project
$ envm set HOGE hoge
$ envm get HOGE
hoge
$ envm ls
HOGE=hoge
$ envm exec env | grep HOGE
HOGE=hoge
```

Variables for `/path/to/project` are saved in `$HOME/.envm/path/to/project/`.

## LICENSE

MIT
