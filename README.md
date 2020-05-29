# Git New

> A cloneable Git template for repeatable and consistent project bootstraps

Inspired by Eric Meyers CSS Reset, Git New is a simple tool to enforce a consistent baseline Git experience for new projects.

- [Git New](#git-new)

  - [For Project Developers](#for-project-developers)
    - [Prerequisites](#prerequisites)
    - [Setup and Configuration](#setup-and-configuration)
  - [For Installers](#for-installers)
    - [Prerequisites](#prerequisites-1)
    - [Setup and Configuration](#setup-and-configuration-1)
  - [Change log](#change-log)
  - [Meta](#meta)
  - [Contributing](#contributing)

## For Developers

Follow this section if you are developing with, installing or deploying this repository.

### Prerequisites

- A good code editor.
### Prerequisites

The versions listed for these prerequisites are current at the time of writing. More recent versions will likely work but "your mileage may vary".

- A good code editor. 
- [Node.js v12.13.0 and NPM 6.14.5](https://nodejs.org/en/download/)
- [Git 2.25+](https://git-scm.com/downloads)

### Setup and Configuration

```sh
# 1. Clone this repository as your new project
git clone git@github.com:tforster/git-new.git /my/path/to/my/project-name

```

### Usage

This repository is intended to serve as a template for new projects by providing a consistent set of control files. Use it by cloning to your new project folder, editing some key properties, re-initialising the .git folder to remove this history and finally replacing the remote with your own.

```sh
# 1. Switch to your new project folder
cd /my/path/to/my/project-name

# 2. Remove the git-new .git database
rm -rf .git

# 3. Install NPM dependencies including linters and code prettiers
npm i

# 4. Edit this README.md and package.json to suit your project
#    - Edit the title to match your project
#    - Edit the description to describe your project

# 5. Edit package.json
#    - Update the title to match the title of this README
#    - Update the description to match the description of this README
#    - Edit the semantic version to match your project requirements

# 6. Delete any unwanted files in /docker (or the entire /docker folder if you're not containerising)

# 7. Re-initialise .git
git init

# 8. Add your own repo's origin
git remote add origin {my-git-origin}

# 9. Update package.json to reflect the new origin and clean up any other properties by following the prompts
npm init

# 10. Delete this instruction block

# 11. Stage and commit files
git add -A
git commit -m"Initial creation"

# 12. Push
git push -u origin master

# 13. Create a develop branch (workflow dependent)
git checkout -b develop
git push -u origin develop

# Your project and repo are ready for your first feature branch
git checkout -b {my-feature-branch-name}
```

## For Project Developers

Follow this section if you will be developing new features and fixing bugs for this repository.

### Prerequisites

- A good code editor. We suggest [VSCode](https://code.visualstudio.com/), [Atom](https://atom.io/) or [SublimeText](https://www.sublimetext.com/).
- [NodeJS LTS+ and NPM 6.14+](https://nodejs.org/en/download/)
- [Git 2.25+](https://git-scm.com/downloads)

### Setup and Configuration

```sh
# 1. Clone this repository as your new project
git clone git@github.com:tforster/git-new.git /my/path/to/my/project-folder/
cd /my/path/to/my/project-folder/git-new

# 3. Create a new branch
git checkout -b {new-branch-name}

# 2. Make changes by editing files and/or using NPM to update dependent packages as well as package.json

# 3. Stage changes
git add -A

# 4. Commit changes
git commit -t"{detailed-commit-message}"

# 5. Push changes
git push origin {new-branch-name}

# 6. Create a pull request
```

## Change Log

See [CHANGELOG.md](changelog.md)

## Meta

Troy Forster – [@tforster](https://twitter.com/tforster) – troy.forster@gmail.com

Distributed under the ISC license. See `LICENSE` for more information.

[https://github.com/tforster/git-new](https://github.com/tforster/git-new)

## Contributing

1. Fork it (<https://github.com/tforster/git-new/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request
