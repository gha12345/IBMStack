

* [Integrating IBM MobileFirst Platform Foundation SDK in Cordova applications](https://mobilefirstplatform.ibmcloud.com/tutorials/en/foundation/7.1/hello-world/integrating-mfpf-sdk-in-cordova-applications/)


* [Integrating IBM MobileFirst Platform Foundation SDK in Cordova applications- Sampple](https://github.com/MobileFirst-Platform-Developer-Center/Cordova/tree/release71)

```bat
NAME
     mobilefirst cordova
SYNOPSIS
     mfp cordova <command> [options]
DESCRIPTION
     IBM MobileFirst Platform Command Line Interface (CLI) for Cordova specific
     actions.
     Specific help for each command is available. For example:
     mfp help cordova create
GLOBAL COMMANDS
     config .............................. View or alter configuration settings
PROJECT COMMANDS
     cordova create .............................. Creates a new Cordova project
     cordova emulate .................................. Emulates Cordova project
     cordova platform ................................ Manages project platforms
     cordova plugin .................................... Manages project plugins
     cordova prepare ............................... Prepares a Cordova project
     cordova preview ......................... Previews existing Cordova project
     cordova run .......................................... Runs Cordova project
COMMAND-LINE FLAGS/OPTIONS
     -v, --version ...............Prints out the version number of this utility
     -d, --debug ........................Debug mode produces a debug log output
     -dd, --ddebug ................... Debug mode produces a verbose log output
EXAMPLE USAGE
     $ mfp cordova create myapp --platform android
     $ cd myapp
     $ mfp cordova preview
     $ mfp cordova emulate --platform android

```


```bat

Warning: using node version v0.12.2 which has been deprecated. Please upgrade to the latest node version available (v6.x is recommended).
Synopsis

cordova command [options]

Global Commands
    create ........ Create a project
    help .......... Get help for a command
    telemetry ..... Turn telemetry collection on or off
    config ........ Set, get, delete, edit, and list global cordova options

Project Commands
    info .......... Generate project information
    requirements .. Checks and print out all the requirements for platforms specified
    platform ...... Manage project platforms
    plugin ........ Manage project plugins
    prepare ....... Copy files into platform(s) for building
    compile ....... Build platform(s)
    clean ......... Cleanup project from build artifacts
    run ........... Run project (including prepare && compile)
    serve ......... Run project with a local webserver (including prepare)

Learn more about command options using 'cordova help <command>'

Aliases
    build -> cordova prepare && cordova compile
    emulate -> cordova run --emulator

Options
    -v, --version ........... prints out this utility's version
    -d, --verbose ........... debug mode produces verbose log output for all activity,
    --no-update-notifier .... disables check for CLI updates
    --nohooks ............... suppress executing hooks (taking RegExp hook patterns as parameters)

Examples
    cordova create myApp org.apache.cordova.myApp myApp
    cordova plugin add cordova-plugin-camera
    cordova platform add android
    cordova plugin add cordova-plugin-camera --nosave
    cordova platform add android --nosave
    cordova requirements android    
    cordova build android --verbose
    cordova run android
    cordova build android --release -- --keystore="..\android.keystore" --storePassword=android --alias=mykey
    cordova config ls
    cordova platform add ios --nofetch
    cordova plugin add cordova-plugin-camera --nofetch
```
