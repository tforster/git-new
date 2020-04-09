# Git New

> A cloneable Git template for repeatable and consistent project bootstraps

Inspired by Eric Meyers CSS Reset, Git New is a simple tool to enforce a consistent baseline Git experience for new projects.

## Installation

Linux, Windows and OSX

```sh
git clone git@github.com:tforster/git-new.git
```

## Usage example

This repository is intended to serve as a template for new projects by providing a consistent set of control files. Use it by cloning to your new project folder, editing some key properties, re-initialising the .git folder to remove this history and finally replacing the remote with your own.

```sh
# 1. Clone this repository as your new project
git clone git@github.com:tforster/git-new.git /my/path/to/my/project-name
cd /my/path/to/my/project-name

# 2. Edit this README.md and package.json to suit your project
#    - Edit the title to match your project
#    - Edit the description to describe your project

# 3. Edit package.json
#    - Update the title to match the title of this README
#    - Update the description to match the description of this README
#    - Edit the semantic version to match your project requirements
#    - Change the Git details including repository, bugs and homepage

# 4. Delete any unwanted files in /docker (or the entire /docker folder if you're not containerising)

# 5. Delete the hidden .git folder created when you cloned
rm -rf .git

# 6. Re-initialise .git
git init

# 7. Add your own repo's origin
git remote add origin my-git-origin

# 8. Delete this instruction block

# 9. Stage and commit files
git add -A
git commit -m"Initial creation"

# 10. Push
git push -u origin master
```

## Development setup

Development setup is very easy. Just clone this repository and start editing.

```sh
git clone git@github.com:tforster/git-new.git
```

## Release History

- 0.1.0 **Initial Creation** (2020-04-09)

Initial creation of this project and Git repository.

## Meta

Troy Forster – [@tforster](https://twitter.com/tforster) – troy.forster@gmail.com

Distributed under the ISC license. See `LICENSE` for more information.

[https://github.com/tforster/git-new](https://github.com/tforster/)

## Contributing

1. Fork it (<https://github.com/tforster/git-newfork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request
