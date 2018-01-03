# Angular Cli plugin for [PHPCI](https://www.phptesting.org)

A plugin for PHPCI to download and install npm packages required by your application.

### Install the Plugin

1. Navigate to your PHPCI root directory and run `composer require robertsobolczyk/phpci-angular-cli`
2. If you are using the PHPCI daemon, restart it
3. Update your `phpci.yml` in the project you want to deploy with

### Prerequisites

1. [angular-cli](https://www.npmjs.com/package/angular-cli) needs to be installed.

### Plugin Options
- **command** _[string, require]_ - Command name. See [docs](https://github.com/angular/angular-cli#usage)
- **directory** _[string, optional]_ - Relative path to run npm-cache in.
- **flags** _[list, optional]_ - Command flags

### PHPCI Config

```yml
    RobertSobolczyk\PHPCI\AngularCli:
        command: build
```
