# Generic New Project Template <!-- omit in toc -->

_A Git template for bootstrapping a variety of projects with a consistent set of control files._

<i>**Template Instructions**

1. Create your new repository by clicking the "Use this template" [button](https://github.com/tforster/git-new/generate) from the GitHub repository. (or download from https://github.com/tforster/git-new/archive/master.zip and unzip)
1. Follow the GitHub prompts to complete the configuration of your new repository
1. Clone your new repository to your local develop environment
1. Install NPM dependencies including linters and code prettiers `npm i`
1. Edit [README.md](README.md)
   - Edit the title to match your project
   - Edit the description to describe your project
   - Edit Prerequisites, Setup and Configuration, Usage, For Users and Meta sections
1. Edit [package.json](package.json)
   - Update the title to match the title of this README
   - Update the description to match the description of this README
   - Edit the semantic version to match your project requirements
1. Update your LICENSE
   - Edit the year and fullname variables in [LICENSE.txt](LICENSE.txt)
   - The provided LICENSE file implements the MIT license as per [https://choosealicense.com/licenses/mit](https://choosealicense.com/licenses/mit)
   - For closed source delete the LICENSE.txt file and update the package.json license property to "UNLICENSED"
   - If neither MIT or UNLICENSED suit your needs consider creating a LICENSE.txt from [https://choosealicense.com/](https://choosealicense.com/)
1. Update [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md). For more information on code of conduct see [https://opensource.guide/code-of-conduct/](https://opensource.guide/code-of-conduct/)
1. Update [CONTRIBUTING.md](CONTRIBUTING.md). For more information about open source contributions see [https://help.github.com/en/github/building-a-strong-community/setting-guidelines-for-repository-contributors](https://help.github.com/en/github/building-a-strong-community/setting-guidelines-for-repository-contributors)
1. Delete any unwanted files in /docker (or the entire /docker folder if you're not containerising)
1. Update [CHANGELOG.md](CHANGELOG.md)
1. Delete this instruction block</i>


- [Prerequisites](#prerequisites)
- [Installation](#installation)
  - [Environment File (.env) Details](#environment-file-env-details)
- [Usage](#usage)
  - [For Local Development](#for-local-development)
  - [To Deploy to Stage or Prod](#to-deploy-to-stage-or-prod)
- [Contributing](#contributing)
- [Change Log](#change-log)

## Prerequisites

The versions listed for these prerequisites are current at the time of writing. More recent versions will likely work but "your mileage may vary".

- A good code editor.
- [Node.js v12.13.0 and NPM 7.0.0](https://nodejs.org/en/download/)
- [Git 2.28](https://git-scm.com/downloads)

## Installation

1. Clone to repository locally, following the directory structure convention:

   ```sh
   git clone git@github.com:tforster/git-new.git \
       ~/dev/{agent}/{client}/{product}/{project}/{component}
   ```

1. Change the current working directory to the new repository directory:

   ```sh
   cd ~/dev/{agent}/{client}/{product}/{project}/{component}
   ```

1. Install dependencies:

   ```sh
   npm install
   ```

### Environment File (.env) Details

Environment files are .gitignored by default since they typically contain sensitive information. This section describes how to manually create an environment file for this project. Note that the .env file is located in the webproducer folder.

  ```ini
  # Comment describing the variable
  VARIABLE=some-value
  ```

## Usage

_Describe the usage here._

### For Local Development

### To Deploy to Stage or Prod

## Contributing

To contribute to this project, please see [`CONTRIBUTING.md`](CONTRIBUTING.md).

## Change Log

To view the release notes for all available versions, please see [`CHANGELOG.md`](CHANGELOG.md).
