oclif-hello-world
=================

oclif example Hello World CLI

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![CircleCI](https://circleci.com/gh/oclif/hello-world/tree/main.svg?style=shield)](https://circleci.com/gh/oclif/hello-world/tree/main)
[![GitHub license](https://img.shields.io/github/license/oclif/hello-world)](https://github.com/oclif/hello-world/blob/main/LICENSE)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g yycu-core
$ cc COMMAND
running command...
$ cc (--version)
yycu-core/2.0.1 linux-arm64 node-v16.20.1
$ cc --help [COMMAND]
USAGE
  $ cc COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`cc help [COMMANDS]`](#cc-help-commands)
* [`cc plugins`](#cc-plugins)
* [`cc plugins:install PLUGIN...`](#cc-pluginsinstall-plugin)
* [`cc plugins:inspect PLUGIN...`](#cc-pluginsinspect-plugin)
* [`cc plugins:install PLUGIN...`](#cc-pluginsinstall-plugin-1)
* [`cc plugins:link PLUGIN`](#cc-pluginslink-plugin)
* [`cc plugins:uninstall PLUGIN...`](#cc-pluginsuninstall-plugin)
* [`cc plugins:uninstall PLUGIN...`](#cc-pluginsuninstall-plugin-1)
* [`cc plugins:uninstall PLUGIN...`](#cc-pluginsuninstall-plugin-2)
* [`cc plugins update`](#cc-plugins-update)
* [`cc update [CHANNEL]`](#cc-update-channel)

## `cc help [COMMANDS]`

Display help for cc.

```
USAGE
  $ cc help [COMMANDS] [-n]

ARGUMENTS
  COMMANDS  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for cc.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.2.19/src/commands/help.ts)_

## `cc plugins`

List installed plugins.

```
USAGE
  $ cc plugins [--json] [--core]

FLAGS
  --core  Show core plugins.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ cc plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v3.5.0/src/commands/plugins/index.ts)_

## `cc plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ cc plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ cc plugins add

EXAMPLES
  $ cc plugins:install myplugin 

  $ cc plugins:install https://github.com/someuser/someplugin

  $ cc plugins:install someuser/someplugin
```

## `cc plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ cc plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ cc plugins:inspect myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v3.5.0/src/commands/plugins/inspect.ts)_

## `cc plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ cc plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ cc plugins add

EXAMPLES
  $ cc plugins:install myplugin 

  $ cc plugins:install https://github.com/someuser/someplugin

  $ cc plugins:install someuser/someplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v3.5.0/src/commands/plugins/install.ts)_

## `cc plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ cc plugins:link PLUGIN

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Links a plugin into the CLI for development.
  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.


EXAMPLES
  $ cc plugins:link myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v3.5.0/src/commands/plugins/link.ts)_

## `cc plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ cc plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ cc plugins unlink
  $ cc plugins remove
```

## `cc plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ cc plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ cc plugins unlink
  $ cc plugins remove
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v3.5.0/src/commands/plugins/uninstall.ts)_

## `cc plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ cc plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ cc plugins unlink
  $ cc plugins remove
```

## `cc plugins update`

Update installed plugins.

```
USAGE
  $ cc plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v3.5.0/src/commands/plugins/update.ts)_

## `cc update [CHANNEL]`

update the cc CLI

```
USAGE
  $ cc update [CHANNEL] [-a] [-v <value> | -i] [--force]

FLAGS
  -a, --available        Install a specific version.
  -i, --interactive      Interactively select version to install. This is ignored if a channel is provided.
  -v, --version=<value>  Install a specific version.
  --force                Force a re-download of the requested version.

DESCRIPTION
  update the cc CLI

EXAMPLES
  Update to the stable channel:

    $ cc update stable

  Update to a specific version:

    $ cc update --version 1.0.0

  Interactively select version:

    $ cc update --interactive

  See available versions:

    $ cc update --available
```

_See code: [@oclif/plugin-update](https://github.com/oclif/plugin-update/blob/v3.2.3/src/commands/update.ts)_
<!-- commandsstop -->
