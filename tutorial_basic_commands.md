# Introduction to Git: a step-by-step guide to your first commit

This tutorial provides a guide, step-by-step, overview of some of Git's basic
commands. Please go through this material **before the start of the course**.

<br>

## 1. Installing and configuring Git

### Installing Git

If you do not have Git installed on your computer, please follow the steps
from the [setting-up your environment](environment_setup.md) instructions.

<br>

### Configuring Git

Before we can use Git, we have to perform a **minimal configuration** setup
that consists in setting your **user name** and **email** address:

```sh
git config --global user.name "First-name Last-name"
git config --global user.email "your.email@example.com"

# Examples:
git config --global user.name "Alice Smith"
git config --global user.email alice.smith@wonder.org
```

To see the config values that are currently set, the commands are the following:
```sh
git config --get user.name
git config --get user.email

# Show all config values at once and where they are set.
git config --list --show-origin
```

Optionally you can also change the **default editor** used by Git, e.g. if you
are more comfortable with `nano` than `vim`:
```sh
git config --global core.editor nano  # Set default editor to nano.
git config --global core.editor vim   # Set default editor to vim (the default).
```

<br>
<br>

## 2. Initializing a new Git repository

```sh
git init
git init <dir to create>
```

<br>
<br>

## 2. Making a commit

### Staging content

```sh
git add

# Shortcuts
git add .
git add --all/-A
git add --update/-u

```

### Making a new commit

```sh
git commit -m "commit message..."
git commit --am "commit message..."
```

<br>
<br>

## 3. History of a Git repo

```sh
git show
git log
```
