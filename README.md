# Git New

_A cloneable Git template for repeatable and consistent project bootstraps_

## Table of Contents

- [Git New](#git-new)
  - [Table of Contents](#table-of-contents)
- [For Developers](#for-developers)
  - [Prerequisites](#prerequisites)
  - [Setup and Configuration](#setup-and-configuration)
  - [Usage](#usage)
- [For Users](#for-users)
- [Change Log](#change-log)
- [Meta](#meta)
- [Contributing](#contributing)
  - [Prerequisites](#prerequisites-1)

# For Developers

Follow this section if you are developing with, installing or deploying this repository.

## Prerequisites

The versions listed for these prerequisites are current at the time of writing. More recent versions will likely work but "your mileage may vary".

- A good code editor.
- [Node.js v12.13.0 and NPM 6.14.5](https://nodejs.org/en/download/)
- [Git 2.25](https://git-scm.com/downloads)

## Setup and Configuration

Clone this repository as your new project.

```sh
git clone git@github.com:tforster/git-new.git /my/path/to/my/project-name
```

## Usage

This repository is intended to serve as a template for new projects by providing a consistent set of control files. Use it by cloning to your new project folder, editing some key properties and re-initialising the .git folder to remove this history and finally replacing the remote with your own.

1. Switch to your new project folder `cd /my/path/to/my/project-name`
1. Remove the git-new .git database `rm -rf .git`
1. Install NPM dependencies including linters and code prettiers `npm i`
1. Edit [README.md](README.md)
   - Edit the title to match your project
   - Edit the description to describe your project
1. Edit [package.json](package.json)
   - Update the title to match the title of this README
   - Update the description to match the description of this README
   - Edit the semantic version to match your project requirements
1. Update your LICENSE
   - Edit the year and fullname variables in [LICENSE.txt](LICENSE.txt)
   - The provided LICENSE file implements the MIT license as per [https://choosealicense.com/licenses/mit](https://choosealicense.com/licenses/mit)
   - For closed source delete the LICENSE.txt file and update the package.json license property to "UNLICENSED"
   - If neither MIT or UNLICENSED suit your needs consider creating a LICENSE.txt from [https://choosealicense.com/](https://choosealicense.com/)
1. Delete any unwanted files in /docker (or the entire /docker folder if you're not containerising)
1. Update [CHANGELOG.md](CHANGELOG.md)
1. Re-initialise .git `git init`
1. Add your own repo's origin `git remote add origin {my-git-origin}`
1. Update package.json to reflect the new origin and clean up any other properties by following the prompts `npm init`
1. Delete this instruction block
1. Stage and commit files `git add -A && git commit -m"Initial creation"`
1. Push `git push -u origin master`
1. Create a develop branch (workflow dependent) `git checkout -b develop && git push -u origin develop`
1. Your project and repo are ready for your first feature branch `git checkout -b {my-feature-branch-name}`

# For Users

Place instructions here if there is some form of installable or runable artifact intended for end users.

# Change Log

See [CHANGELOG.md](changelog.md)

# Meta

Troy Forster – [@tforster](https://twitter.com/tforster) – troy.forster@gmail.com

See [LICENSE](LICENSE.md) for more information.

[https://github.com/tforster/git-new](https://github.com/tforster/git-new)

# Contributing

This section applies if you will be developing new features and fixing bugs for this repository.

```sh
# Fork it from GitHub https://github.com/tforster/git-new/fork

# Create your feature branch
git checkout -b {meaninful-branch-name}

# Commit your changes
git commit -a"{meaninful commit message}"

# Push to the branch
git push origin {meaninful-branch-name}

#Create a new Pull Request
```

## Prerequisites

The prerequesites for contributing to this repo are the same is if you were developing with it.

- A good code editor.
- [Node.js v12.13.0 and NPM 6.14.5](https://nodejs.org/en/download/)
- [Git 2.25](https://git-scm.com/downloads)
