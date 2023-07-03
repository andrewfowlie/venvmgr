# venvmgr

_👀 Manage Python virtual environments_

A command line application to manage Python virtual envionrments (venvs). 

Create a venv:

```bash
$ vm create example
```
Use it:

```bash
$ vm python --venv example code.py
```

The assoications between files and venvs is recorded, such that

```bash
$ vm python code.py
```

uses the `example` venv. We might want install packages in this venv, e.g.,

```bash
$ vm pip --venv example scipy
```

We now might want to check the venvs:

```bash
$ vm ls
example
created at 2023-07-03 12:07:48.872147
activate: source /home/user/.venvmgr/example/bin/activate
used by: /home/user/code.py
```

Lastll, we might want to activate this venv

```bash
$ vm activate example
```

## Install 💥

```bash
pipx install venvmgr
```
